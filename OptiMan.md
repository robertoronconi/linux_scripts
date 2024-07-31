#!/bin/bash
	echo
	echo
	echo "--- Basado en: uCare System Core https://github.com/Utappia/uCareSystem"
sleep 1
    echo
echo -
	echo "#########################"
	echo        "     Comencémos!"
	echo "#########################"
	sleep 1
echo -
	echo "#########################"
	echo      "     A limpiar un poco !"
	echo "#########################"
echo -
sleep 5
sudo apt autoremove -y; sudo apt autoclean; sudo apt clean; sudo aptitude clean; sudo aptitude autoclean; sudo du -sh  /var/cache/apt; sudo apt-get install deborphan; sudo deborphan | xargs sudo apt-get -y remove --purge;
echo
  	echo "#########################"
	echo        "     A actualizar !"
	echo "#########################"
	 echo
sudo aptitude update; sudo snap refresh; sudo flatpak update -y; sudo apt full-upgrade -y; sudo apt upgrade -y; sudo apt-get dist-upgrade; sudo apt install -f;  sudo dpkg --configure -a;  sudo apt --fix-broken install; sudo nala update; sudo nala upgrade;
    echo
 echo "- Algunos complementos
– Nala (front-end APT) https://gitlab.com/volian/nala
– Czkawka https://github.com/qarmin/czkawka   
– Bleachbit https://www.bleachbit.org/
– Stacer https://oguzhaninan.github.io/Stacer-Web/  
– Cylondeb https://github.com/gavinlyonsrepo/cylon-deb "
echo
    echo "#########################"
    echo "Todo listo... Hasta luego"
    echo "#########################"
exit 0
fi
