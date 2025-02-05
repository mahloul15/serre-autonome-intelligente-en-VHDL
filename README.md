Composants du projet
Capteur de température  : mesure la température pour activer le module Peltier et le ventilateur.
Capteur d'humidité du sol : détermine quand activer la pompe d'arrosage.
Actionneurs :
Module Peltier + ventilateur :
Mode chauffage si température trop basse.
Mode refroidissement si température trop haute.
LED horticole :
Fournit de la lumière si l’éclairage naturel est insuffisant.
Pompe à eau :
Arrose la plante si le sol est trop sec.
Fonctionnement général
Capteur	Action
Température élevée	Activer Peltier (mode refroidissement) + ventilateur
Température basse	Activer Peltier (mode chauffage)
Sol sec	Activer pompe à eau
Lumière insuffisante	Activer LED horticole
Tout cela sera automatisé en VHDL.
Code VHDL : Architecture du projet
Le projet peut être découpé en plusieurs modules :

Module de gestion des capteurs

Lire la température et l’humidité.
Comparer les valeurs aux seuils définis.
Module de contrôle des actionneurs

Allumer/éteindre le Peltier, ventilateur, LED, pompe en fonction des valeurs lues.
Module de régulation intelligente

Gérer la transition entre chauffage/refroidissement et irrigation pour ne pas abîmer la plante.
