# gps_pas_cher
un gps tout simple avec une arduino nano.

Vous voulez un gps capable simplement de donner votre latitude, longitude, vitesse en km/h et en noeuds,l' heure utc sans traceur ou fonctions annexes (waypoints, prévisionnel, optimisation de route, faire le café), mais avec un budget au final équivalent à une trentaine d'euros ? Alors vous êtes bien tombé !

Matériel:
-GPS NEO-7M avec son antenne (arduino)
-arduino nano
-ecran oled ssd1306 128 pixels sur 64
-boitier de dérivation, ou autre pour faire le boitier
-pile 9 volts
-interrupteur

Il faut attendre entre dix et soixante secondes pour la mise en route du gps à l'allumage, le temps de capter les satellites.

Photos:

![20231108_141804](https://github.com/HarryTutle/gps_pas_cher/assets/82940602/11414494-3527-4cc2-8810-aadb01135efb)

![20231108_141756](https://github.com/HarryTutle/gps_pas_cher/assets/82940602/298b1a53-c473-42ae-88cc-88ae3718ce71)

![20231108_141750](https://github.com/HarryTutle/gps_pas_cher/assets/82940602/6f3e642f-24ad-4588-9c55-1ca126b983ca)


Je n'ai pas mis de schéma fritzing, le montage est assez simple. La pile 9 volts se branche sur les bornes vin et ground de l'arduino, l'alimentation du gps se branche sur le 5v de l'arduino et ground, rx et tx respectivement les bornes 3 et 4 (liaison série). Pour l'écran oled c'est une liaison i2c, donc sda se branche sur la borne A4 et scl sur la borne A5.L'ecran peut fonctionner sur du 3.3 volts.
