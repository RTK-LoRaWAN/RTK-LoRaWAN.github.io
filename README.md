# RTK LoRaWAN : RTK over LoRaWAN

La [Cinématique temps réel (Real Time Kinematic, en anglais ou RTK)](https://docs.centipede.fr/docs/centipede/2_RTK.html) est une technique de positionnement par satellite basée sur l’utilisation de mesures de la phase des ondes porteuses des signaux émis par les systèmes GPS, GLONASS ou Galileo. Une station de référence fournit des corrections en temps réel permettant d’atteindre une précision de l’ordre du centimètre. Autrefois très couteux (plusieurs milliers d’euros), une station de référence peut être assemblée pour quelques centaines d’euros avec la dernière génération de modules GNSS centrimêtrique comme le [module uBlox RTK ZED-F9P](https://www.u-blox.com/en/product/zed-f9p-module). Les positions GPS des stations fixes (ainsi que les écarts à la position réélle) sont collectées par un “caster” qui diffusent celles-ci auprès de systemes nomades (véhicules agricoles, voitures autonomes, drones, surveillance d’infrastructure comme des ponts et de barrages,, mouvements de glaciers ou de falaises, secours et catastrophes naturelles, contributeurs à OpenStreetMap …) aussi appelé Rovers. En France, il existe un réseau collaboratif de stations de référence : https://centipede.fr/ .

Actuellement, la récupération des massages (par les Rovers) passent par l’utilisation de connection IP (en liaison 3G/4G).

Il existe des technologies de communication dite longue distance (long range) et basse consommation (low power) comme [LoRa/LoRaWAN](https://fr.wikipedia.org/wiki/LoRaWAN) qui peuvent être utilisés pour diffuser les messages correctifs du zone circonscrite (~30-60 Kms carré) pour diffuser les messages RTK avec une faible coût énergétique et vers des objets qui ne disposent pas d’une liaison 3G/4G ou qui sont en zone blanche (ie sans réseau terrestre opéré).

L'objectif du projet est développer des solutions de station de référence RTK et de rovers s'appuyant sur LoRaWAN pour diffuser (ie "caster") les messages RTK.

Un premier test est prévu sur Grenoble et alentours en contribuant au réseau de stations de référence RTK de https://centipede.fr/

## Projets étudiants
* [ENSIMAG 2A 2022](https://fablab.ensimag.fr/index.php?title=Station_de_base_et_rovers_GPS_centrim%C3%A9trique_avec_transmission_LoRa)
