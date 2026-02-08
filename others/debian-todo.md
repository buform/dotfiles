0. WAŻNE PLIKI
	* fstab
		/etc/fstab

	* sources list
		etc/apt/sources.list

	* grub
		/etc/default/grub

1. AKTUALIZACJA I DEZAKTUALIZACJA
	sudo apt update && sudo apt upgrade -y && sudo apt dist-upgrade -y && sudo apt autoremove -y && sudo apt install -y lsb-release
	
2. FIRMWARE LINUX
	sudo apt install firmware-linux firmware-linux-nonfree firmware-misc-nonfree
	
3. INNY FIRMWARE
	sudo apt install firmware-realtek firmware-atheros
	
4. STEROWNIKI KARTY GRAFICZNEJ
	* NVIDIA
		sudo apt install nvidia-detect
		sudo nvidia-detect
		sudo apt install nvidia-driver nvidia-settings


	  * AMD
		sudo apt install libdrm-amdgpu1 xserver-xorg-video-amdgpu
		sudo apt install mesa-vulkan-drivers libvulkan1 vulkan-tools vulkan-validationlayers

5. FIRMWARE BROADCOM
	sudo apt install broadcom-sta-dkms broadcom-sta-common firmware-brcm80211 firmware-iwlwifi
	
6. BLUETOOTH
	sudo apt install bluetooth bluez bluez-firmware bluez-cups bluez-tools firmware-iwlwifi blueman
	sudo systemctl enable bluetooth
	sudo systemctl start bluetooth
	sudo vim /etc/bluetooth/main.conf

	
7. MIKROKOD DO PROCESORÓW (SYSTEM AUTOMATYCZNIE INSTALUJE PODCZAS STANDARODWEJ INSTALACJI)
	* INTEL
		sudo apt install intel-microcode

	* AMD
		sudo apt install amd64-microcode
		
8. AUTOMATYCZNE WYSZUKIWANIE FIRMWARE
	sudo apt install isenkram-cli
	sudo isenkram-autoinstall-firmware

9. 32-BIT WINE
	sudo dpkg --add-architecture i386
	
10. KODEKI
	sudo apt install ffmpeg rar unrar libavcodec-extra ttf-mscorefonts-installer
	
11. GRUB
	sudo nano /etc/default/grub
	sudo update-grub
 	Czas uruchomienia 1 sekunda. Przy zmiennej quiet dać ```splash```.

12. LAPTOPY - ZARZĄDZANIE ENERGIĄ
	sudo apt install tlp tlp-rdw
	sudo tlp start
	sudo tlp start

13. USTAWIENIA I PODSTAWOWE NARZĘDZIA
	sudo apt install mc inxi git htop bpytop bat mughsot menulibre cmatrix lightdm-gtk-greeter-settings fonts-noto-color-emoji thunar-archive-plugin cifs-utils gvfs-backends wireless-tools net-tools redshift-gtk

	* gufw - zapora sieciowa
	* mpv - odtwarzacz mulitmedialny
	* audacious - odtwarzacz muzyki
	* geany - odpowiednik Notepad++
	* kolourpaint - odpowiednik Paint
	* geepie - przeglądarka plików graficznych

14. DRUKARKA HP STEROWNIKI
	 * hplip
	 * hplip-gui
	
15. WTYCZKI XFCE4 (SĄ ZAWARTE W PAKIECIE ```xfce4-goodies```)
	* xfce4-cpufreq-plugin
	* xfce4-cpugraph-plugin
	* xfce4-sensors-plugin
	* xfce4-systemload-plugin
	* xfce4-battery-plugin
	* xfce4-power-plugin
	
16. WYGLĄD
	* papirus-icon-theme
	* orchis-gtk-theme
	
17. FLATPAK
	sudo apt install flatpak
	sudo flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo

	Jeśli masz środowisko GNOME to:
	sudo apt install gnome-software-plugin-flatpak
	
18. ARDUINO BRAK ZEZWOLENIA NA PORT
	sudo usermod -a -G dialout username

19. LIBREOFFICE INSTALACJA CAŁEGO PAKIETU
	sudo apt install libreoffice lsb-release libreoffice-style* libreoffice-gtk3 libreoffice-l10n-pl libreoffice-help-pl hunspell-pl myspell-pl
	
20. USUWANIE PROGRAMÓW
	sudo apt remove libreoffice-*
	sudo apt remove exfalso quodlibet
	
21. KOMENDY APT USUWANIE
	* usuwanie danego pakietu
		sudo apt remove package

	* usuwanie nieużywanych pakietów
		sudo apt autoremove

	* czyszczenie po instalacji
s		sudo apt autoclean
	
2. DODANIE REPOZYTORIUM NON-FREE I CONTRIB
	sudo apt install software-properties-common -y
	sudo apt-add-repository contrib non-free

	LUB
		
	sudo vim /etc/apt/sources.list
	CONTRIB i NON-FREE do każdego

23. ŚRODOWISKO GRAFICZNE XFCE4
	sudo apt install xfce4 lightdm

24. REDSHIFT CONFIG FILE
[redshift]
temp-day=5700
temp-night=3600
;brightness=0.9
;gamma=0.8
location-provider=manual
;location-provider=geoclue2

[manual]
lat=52.22
lon=21.01

25. WINE
	https://wine.htmlvalidator.com/install-wine-on-debian-12.html

26. SPOTIFY
	https://www.spotify.com/pl/download/linux/

27. INNE OPROGRAMOWANIE
	* gnumeric
	* claws-mail
	* pidgin
	* catfish
	* asunder

28. 
