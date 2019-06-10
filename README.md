# VERSION ACTUALIZADA CON TECLADO INLINE


Es la version modificada que yo uso del teclado inline del dtgbot con las correcciones que el creador ha hecho al branch master y el idioma español. 

CONSEJO DTGBOT: No usar acentos ni ñ en los nombres de dispositivos para que DTGBOT no se cuelgue al intentar usarlos. Creo que pasa en todas las versiones no solo en la inline.


# INSTALACION DESDE CERO

 Para una INSTALACACION DESDE CERO, sigue los pasos de: https://www.domoticz.com/wiki/Remote_Control_of_Domoticz_by_Telegram_Bot hasta el final, solo cambia la direccion del DTGBOT para bajar mi version inline.
 
 
en vez de:

git clone https://github.com/steps39/dtgbot.git
ejecutamos 2 comandos: 

git clone https://github.com/victordz/dtgbotesp.git

mv dtgbotesp dtgbot

## [LIBRERIA NECESARIA, SINO DARA ERROR]## (si la version 8u11 cambia este enlace no servira, buscar nuevo)

wget http://security.debian.org/debian-security/pool/updates/main/o/openssl/libssl1.0.0_1.0.1t-1+deb8u11_armhf.deb

sudo dpkg -i libssl1.0.0_1.0.1t-1+deb8u11_armhf.deb


## SI YA TIENES DTGBOT EN MARCHA PERO QUIERES PROBAR ESTE MENU INLINE:
SOLO SI YA VIENES CON DTGBOT instalado y unicamente quieres probar este menu inline, tienes que seguir esta pequeña fraccion de las instruciones:

Copia de seguridad de tu dtgbot actual para poder deshacer todo:

sudo service dtgbot stop

cd ~

mv dtgbot olddtgbot


Instalacion de este DTGBOT inline:

cd ~

git clone https://github.com/victordz/dtgbotesp.git

mv dtgbotesp dtgbot

cd ~/dtgbot

chmod 755 dtgbot

chmod 755 *.sh

cd ~/dtgbot/bash

chmod 755 *.sh

Como el resto ya estaba instalado, solo falta arrancarlo:

sudo service dtgbot start

# Inline DTGMenu screenshots:</b>
  ![Alt text](/img/Inline-menus.jpg?raw=true "DTGMenu")
