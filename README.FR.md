# TeleInfo - ST32WB55

[English version / Version anglaise](README.md)

Ce projet permet de récupérer les informations des compteurs Linky (et ancien compteurs) via les bornes de télé-information clients et les transmettres en Zigbee. Le module s'alimente via l'alimentation de 150mW dédié des Linky.


Ce dépot comporte les sources Kicad de la PCB et les sources du Firmware.


## PCB

La carte PCB est basé sur :
* Un microcontroller [STM32WB55CCU6](https://www.st.com/en/microcontrollers-microprocessors/stm32wb55cc.html) qui se charge de la récupération des informations et de la retransmission en zigbee
* Un pont de diode pour la conversion de l'alimentation en courant alternatif du linky en courant continue.
* Un regulateur lineaire LM2937-IMP pour la conversion en 3.3V
* Un octocoupleur SHA620-A pour la récupération de liason serie de la TeleInfo
* 2 broche d'alimentation 5V (5V et GND) pour les anciens compteurs. Avec un jumper pour le choix entre Linky/5V
* 5 broche pour flasher le microcontroller avec un st-link (SWD).








