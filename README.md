# kvantovecytochromy
## Vizualizácia
V prvej úlohe (notebook [KvantCHE_diclofenac.ipynb](https://github.com/hruska-lab/kvantovecytochromy/blob/main/KvantCHE_diclofenac.ipynb)) sme sa zamerali na [2D](https://github.com/hruska-lab/kvantovecytochromy/blob/9ad385314a003fb5ff40a05b1076357d781a9c84/diclofenac-2D.png) a [3D](https://github.com/hruska-lab/kvantovecytochromy/blob/9ad385314a003fb5ff40a05b1076357d781a9c84/diclofenac-3D.png) vizualizáciu molekuly Diclofenac. Obrázky sme uložili vo formáte .png.

V druhej úlohe (notebook [Diclofenac_in_water.ipynb](https://github.com/hruska-lab/kvantovecytochromy/blob/main/Diclofenac_in_water.ipynb)) pomocou aplikácie ForceField v Colabe vytvorili [simuláciu](https://github.com/hruska-lab/kvantovecytochromy/blob/main/Diclofenac_in_water.ipynb) molekuly diklofenaku vo vode s [500](https://github.com/hruska-lab/kvantovecytochromy/blob/main/trajectory.pdb) (vo fotmáte .pdb) aj [100 000](https://github.com/hruska-lab/kvantovecytochromy/blob/main/trajectory_100000.dcd) (vo fotmáte .dcd) krokmi, [dáta](https://github.com/hruska-lab/kvantovecytochromy/blob/main/data.csv) zo simulácie aj trajektóriu molekuly sme uložili a vizualizovali sme ju pomocou [Pymol](https://github.com/hruska-lab/kvantovecytochromy/commit/63067759b46ddd889813904cf1b509b0893b174e) vo vodnom prostredí aj bez vodného prostredia.

V tretej úlohe (notebook [PyEMMA_1.ipynb](https://github.com/hruska-lab/kvantovecytochromy/blob/main/PyEMMA_1.ipynb)) sme pomocou PyEMMA vytvorili [grafy](https://github.com/hruska-lab/kvantovecytochromy/blob/main/PyEMMA_1.ipynb) zobrazujúce distribúcie konformácii molekuly diklofenaku po redukcii dimenzii.

V štvrtej úlohe (notebook [PyEMMA_2.ipynb](https://github.com/hruska-lab/kvantovecytochromy/blob/main/PyEMMA_2.ipynb)) sme pomocou PyEMMA vytvorili grafy hustoty konformácii diklofenaku, v ktorých sme označili lokálne [minimá](https://github.com/hruska-lab/kvantovecytochromy/commit/7c6d97e5b0662b8e4d6b3af857f54063d3c6cedd). Tieto minimá sme následne uložili vo formáte .pdb aj vo formáte [.xyz](https://github.com/hruska-lab/kvantovecytochromy/commit/ac0c734bcdacdcbd3212659872dd5f828fa4add7) a [vizualizovali](https://github.com/hruska-lab/kvantovecytochromy/commit/6d4ff7c742b7a85b2574faf6b3a8dcbe1afee37b) sme ich (formát .pdb) v Pymol. Vizualizácie miním sme porovnali s [predošlými](https://github.com/hruska-lab/kvantovecytochromy/commit/c8244dedf33f060e13fd14489c6c84e6454145f0) trajektóriami.

V piatej úlohe (notebook [Tutoriál_01_Energy_Convergence.ipynb](https://github.com/hruska-lab/kvantovecytochromy/blob/main/Tutori%C3%A1l_01_Energy_Convergence.ipynb)) sme upravili tutoriál pre diklofenak a vypočítali sme tak Hartree-Fock a Density Functional Theory energie. Vďaka tutoriálu 00_PySCF_Intro.ipynb sme vytvorili [cube view.png](https://github.com/hruska-lab/kvantovecytochromy/blob/main/cube%20view.png), teda niečo ako zobrazenie elektrónovej hustoty diklofenaku.

V šiestej úlohe (notebook [Rozdiely_01_Energy_Convergence.ipynb](https://github.com/hruska-lab/kvantovecytochromy/blob/main/Rozdiely_01_Energy_Convergence.ipynb)) sme vypočítali rozdiely jednotlivých energií (Hartree-Fock, Density Functional Theory a Møller–Plesset perturbation theory) medzi diklofenakom so všetkými vodíkmi a diklofenakom, ktorému chýbal jeden z vodíkov. Toto sme urobili pre každý z 11 vodíkov prítomných v diklofenaku. Vypočítané rozdiely sme zapísali do dokumentu [KvantChe_energie.docx](https://github.com/hruska-lab/kvantovecytochromy/blob/main/KvantChe_energie.docx).

V siedmej úlohe (notebook [Diklofenak_číslovanie.ipynb](https://github.com/hruska-lab/kvantovecytochromy/blob/main/Diklofenak_%C4%8D%C3%ADslovanie.ipynb)) som vytvorila program na očíslovanie atómov vodíka v molekule diklofenaku (z predtým získaných dát [new_localmin_1.xyz](https://github.com/hruska-lab/kvantovecytochromy/blob/main/new_localmin_1.xyz) o tejto molekule). V článku https://pubs.acs.org/doi/epdf/10.1021/ja402016p autori dospeli k záveru, že C5 je chemicky preferovaným miestom oxidácie diklofenaku. V našom číslovaní molekuly diklofenaku by tento záver znamenal, že H1 je vodík, ktorý sa najľahšie odštiepi. Z našich predošlých zistení ale vieme, že hodnota rozdiel_DFT je najväčšia pre H9, teda diklofenak bez H9 má najnižšiu energiu. Naopak hodnota rozdiel_DFT je najmenšia pre H3, teda diklofenak bez H3 má najvyššiu energiu.
