# Cam87circle
**Cam87 Redux** un capteur APS-C dans le corps d'une cam planétaire ZWO

** PRELIMINARY COMMIT **
** not validated **

![ED view](https://github.com/zUrp-Astronomics/Cam87-Redux/blob/c6d6775af85cb11b0b84bf59b08a4f8a324bd49f/Logic_board/Cam87R_edux%20-%20Logic_board_v1.1%20-%202_3D-view_top.png)

OSHWlab project : https://oshwlab.com/lordzurp/cam87_redux

**la base**
la Cam87, c'est un projet ukrainien du turfu pour faire une caméra astro refroidie à partir d'un capteur de Nikon D40 : APS-C, 6Mpx, 7.8µm
(c'est le même capteur dans les QHY 8Pro https://www.astroshop.de/fr/cameras-astronomiques/camera-qhy-8-pro-color/p,54748#specifications

j'ai déjà une version "box" fonctionnelle, donc on part d'un projet déjà validé, mais la méccanique était à revoir (3 PCBs à assembler, boitier imprimé fragile ...)

**le projet**
rentrer ce truc dans le boitier d'une caméra planétaire ZWO
j'ai un boitier de asi224 vide (électronique fumée), techniquement ça doit passer !

**Updates schéma**
- refonte de la partie refroidissement : opto-coupleur et MosFET isolé du reste du PCB
- ajout de capa de découplage un peu partou
- reprise de la BOM pour optimiser le coût et le placement (-> 0402 ...)
- retour sur une EEPROM standard (merci la dispo)

**PCB**
- rond, 56mm de diamètre
- zone de composants 48.5mm (rebord interne du boitier)
- séparation au max des parties alim, ADC, pilotage CCD H et V, logique
- découplage des alims aux ptis oignons, des capa partout où ya un trou
- connecteur USB type B

**Version alternative**
- rond de 48.5mm diamètre
- connecteur USB-C
- pas de MosFET, jsute l'opto pour le refroidissement


**Fabrication**
pour 5 cartes, c'est 160€, donc environ 200€ au final => 40€ pièce

