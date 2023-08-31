## Bendrieji užduočių reikalavimai:

* Balas:
  * Už užduotį galima gauti daugiausia 4/3 balų.
  * Už pavėluotą pateikimą bus atimama po 1/3 balo per savaitę.
* Užduotys:
  * Užduotis galima gauti per pratybas.
* Pakartotiniai atsiskaitymai:
  * Jei užduotis nėra tinkamai atlikta arba jos nepavyko išspręsti, jums gali būti leista ją pataisyti ar iš naujo išspręsti šių ar kitų pratybų metu. Tai suteikia jums galimybę ištaisyti savo klaidas.
  * Vėlavimas fiksuojamas rašant balą.
* Atsiskaitymas ir vertinimas:
  * Atsiskaitymai priimami tik pratybų metu.
  * Atsiskaitymuose turi dalyvauti visi autoriai.
* Reikalavimas egzaminui:
  * Egzaminą/įskaitą galite laikyti tik surinkę bent 1 balą iš užduočių.
* Savarankiškas darbas:
  * Visos užduotys turi būti parašytos savarankiškai.
* Derinimas su dėstytoju:
  * Galite sugalvoti ir pasiūlyti savo užduotį.
  * Pasirenkamą užduotį reikia suderinti su pratybų dėstytoju ir registruoti likus ne mažiau kaip savaitei iki atsiskaitymo.
* Teisingas funkcionalumas:
  * Atlikta užduotis turi veikti tinkamai, nesugriūti ir tinkamai apdoroti visus duomenis.
* Atsiskaitymo metu turite:
  * Parodyti savo programos veikimą.
  * Gebėti paaiškinti savo kodą ir jo logiką.
  * Atsakykite į visus papildomus dėstytojo klausimus.
  * Jei reikia, būkite pasirengę pakeisti savo programą.

## Pirma užduotis

* Skriptas turi atitikti Unix programavimo principus ir imituoti kitų Unix programų elgesį. Jis turėtų būti neinteraktyvus ir veikti taip, kad atitiktų Unix komandinės eilutės priemones.
* Skripto išvestis turi būti paprasto ir standartizuoto formato, kad vartotojai galėtų lengvai įtraukti išvestį į kitas Unix programas ar konvejerius.
* Jei scenarijui reikalingi įvesties arba konfigūracijos parametrai, jie turėtų būti priimti kaip komandinės eilutės argumentai arba nuskaityti iš standartinės įvesties (stdin).
* Venkite laikinųjų failų naudojimo ir failų kūrimo bei įrašymo į failus, imkitės šių veiksmų tik tada, kai nėra kitos tinkamos galimybės.
* Kai tik įmanoma, atlikite duomenų apdorojimą naudodami konvejerius (`|`), kad sujungtumėte kelis procesus.
* Nenaudokite kintamųjų, ciklų ir sąlygos sakinių, nebent nėra kitos tinkamos galimybės.
* Skriptas turi būti suderinamas su `/bin/sh` ir neturėtų pasikliauti funkcijomis ar sintaksėmis, būdingomis kitiems apvalkalams, pvz., `/bin/bash` arba `/bin/tcsh`.
* Skriptas negali naudoti aukšto lygio programavimo kalbų arba nuo jų priklausyti; jis turėtų būti parašytas tik naudojant apvalkalo programas ir vengti išorinių priklausomybių nuo kalbų, tokių kaip Python, Perl ar Ruby.

[Pirmosios užduoties pavyzdžiai](Pirmosios-užduoties-pavyzdžiai.md)

## Antra užduotis

Šios užduoties tikslas – parodyti tvirtą supratimą apie darbą su Unix procesais naudojant C programavimo kalbą. Programa turi sąveikauti su procesais, priimti ir apdoroti komandas bei atitikti toliau nurodytus reikalavimus:

* Parašykite savo kodą C programavimo kalba.
* Į kodą įtraukite pakankamai komentarų, kad būtų aiškiau ir paaiškintumėte savo logiką bei požiūrį.
* Įsitikinkite, kad kodas gali veikti universiteto Linux kompiuteryje.
* Sukurkite funkcinį Makefile savo programai ir įsitikinkite, kad kodas gali būti sukompiliuotas naudojant jį.
* Paleidę programą, parodykite vartotojui kviečiantį pranešimą.
* Programa turi priimti ir apdoroti vartotojo komandas.
* Programa baigiama vienu iš šių būdų:
  * Gavęs EOF (failo pabaiga).
  * Gavęs iš vartotojo komandą "exit".
* Nenaudokite `system(3)` funkcijos komandoms vykdyti.
* Naudojant tik standartines Unix API funkcijas, tokias kaip `fork(2)`, `execv(2)`, `exit(2)`, ...
* Procesų valdymui nenaudoti išorinių bibliotekų.
* Pasirinkite vieną iš šių reikalavimų:
  1. konvejeriai

     Realizuokite konvejerių palaikymą, kad vieno proceso išvestis būtų naudojama kaip kito proceso įvestis. Pavyzdžiui, vartotojai turėtų turėti galimybę vykdyti tokias komandas kaip `command1 | command2` perduoti `command1` išvestį kaip įvestį `command2`.

  2. foninis apdorojimas

     Realizuokite apdorojimą fone pagal UNIX `/bin/sh` apvalkalą (shell), realizuodami komandas `bg`, `fg`, `kill` valdymo operatorių `&`.

  3. srautų nukreipimas

     Realizuokite srautų nukreipimo funkcionalumą pagal UNIX `/bin/sh` apvalkalą (shell), jame nukreipimai atliekami naudojant operatorius `>`, `>>`, `<`, `n>`, ...
* Pastaba: nereikia realizuoti išorinių programų, tokių kaip `ls(1)`, `sort(1)` ar `grep(1)`. Vietoj to turėtumėte iškviesti šias programas naudodami tokias funkcijas kaip `execv(2)`.

## Trečia užduotis

Šios užduoties tikslas – parodyti savo žinias ir įgūdžius dirbant su lizdais naudojant BSD socket API C programavimo kalba. Sukurkite C programą, kuri naudoja lizdus, vienu metu aptarnauja kelis klientus ir naudoja įvairias su lizdais susijusias funkcijas.

* Programa turi naudoti šias su lizdais susijusias funkcijas iš BSD socket API:
  * `select(2)`, `socket(2)`, `send(2)`, `recv(2)`, `close(2)`, `shutdown(2)`, `accept(2)`, `listen(2)`, `bind(2)`, `connect(2)`.
  * Tinklo vardų išrišimo funkcijas
  * `hton*(2)`, `ntoh*(2)` funkcijos (Pastaba: jų galima nenaudoti tik tuo atveju, jei jų nebuvimas neturi įtakos programos teisingumui).
  * Kelių klientų palaikymas: programa turėtų būti pajėgi aptarnauti kelis klientus vienu metu. Tai reiškia, kad ji turėtų turėti galimybę vienu metu dirbti su keliais klientais, neblokuodama kitų klientų.
  * Nenaudokite išorinių bibliotekų darbui su lizdais. Programa turėtų naudoti tik BSD socket API funkcijas.
  * Labai svarbu, kad gerai suprastumėte savo kodą ir galėtumėte paaiškinti, kaip jis veikia. Taip pat turėtumėte sugebėti paaiškinti, kaip veikia kode naudojamos BSD lizdo API dalys ir prisideda prie bendro programos funkcionalumo.
  * Architektūra:
    * Kliento ir serverio architektūra, realizuotkite kliento ir serverio programas.
    * Peer-to-Peer (P2P) architektūra.

[Kurso teorijos konspektas](konspektas.pdf)

[os-unix](https://bit.ly/os-unix)
