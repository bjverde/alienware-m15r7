# :alien: Alienware M15 R7 :computer: with Linux :penguin:
How to config :alien: Alienware M15 R7 :computer: with Linux :penguin: Ubuntu Studio 22.04 LTS 

Alienware with other hardware:
* UGreen 9-in-1 USB-C Hub
* LG HDMI external monitor
* External VGA LG monitor connected to Ugreen
* Logitech MX Keys keyboard connected to Ugreen
* Logitech mouse connected to Ugreen
* wired network connected to Ugreen

See this documentation in other languages:
- :us: [English version](README_en.md)
- :brazil: [Portuguese version available](README.md). This is main documentation. This translates to the other languages

<img src="assets/dell-alienware-m15-r7.jpg" width=600 height=600 alt="Notebook Dell AlienWare M15 R7">

<img src="assets/ugreen_hub_usb-c-9in1.jpg" width=300 height=300 alt="Hub USB-C 9in1">

Como configurar o notebook Dell :alien: Alienware M15 R7 :computer: com Linux :penguin: Ubuntu Studio 22.04 LTS, a interface grafica de referencia ẽ o KDE Plamas

Alienware com outros hardwares:
* Hub USB-C UGreen 9 em 1
* Monitor externo LG HDMI
* Monitor LG externo VGA ligado no Ugreen
* teclado Logitech MX Keys ligado no Ugreen
* mouse Logitech ligado no Ugreen
* rede cabeada ligado no Ugreen


# 1 - Faça um pendrive de instalção de segurança
https://www.dell.com/support/kbdoc/pt-br/000125230/how-to-create-and-use-the-dell-recovery-restore-usb-drive

# 2 - Altere a configuração da BIOS 
https://www.dell.com/support/kbdoc/pt-br/000148406/alienware-sistemas-baseados-em-ubuntu-disable-secure-boot-to-modify-ou-replace-o-carregador-de-inicializa%C3%A7%C3%A3o

# 3 - Update Kernel to 5.18
Instruções baseado no https://linuxhint.com/install-upgrade-latest-kernel-ubuntu-22-04/

Atuliazar pacotes e verificar Kernel instalado
```bash
sudo apt update; uname -mrs;
```

Adcionando novo respositorio e instalado gerenciador de Kernels
```bash
sudo add-apt-repository ppa:cappelikan/ppa -y; sudo apt install mainline -y
```

# 4 - Install NVidia Drive
Install NVIDIA Drivers on Ubuntu 22.04 LTS
https://linuxhint.com/install-nvidia-drivers-on-ubuntu/

# 5 - Install Wireless
https://askubuntu.com/questions/1439264/no-wi-fi-adapter-found-on-ubuntu-22-04-on-alienware-m15-r17


# 6 - Sugestoes de software adicionais
```bash
sudo apt-get update -y;sudo apt-get install -y kde-spectacle
```
# 7 - Configurar mais de um layout de teclado 

<img src="assets/teclado.png" width=300 height=300 alt="layout keyboard kde plasma">


# 8 - Install ddcci-plasmoid
KDE Plasma Widget for external monitor brightness adjustment
https://github.com/davidhi7/ddcci-plasmoid
