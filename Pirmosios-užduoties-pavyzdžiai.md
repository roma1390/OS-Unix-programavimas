* Lankomiausi puslapiai: parašykite skriptą, kuris analizuoja `access_log` failą ir identifikuoja `N` dažniausiai lankomus puslapius bei jų kiekį.
* Naršyklių statistika: sukurkite skriptą, kuris analizuoja `access_log` failą ir generuoja statistiką apie dažniausiai naudojamas naudotojo naršykles pasiekiančias svetainę.
* HTTP būsenos kodo (status code) ataskaita: parašykite skriptą, kuris nuskaito `access_log` nurodytą būsenos kodą `C` ir generuoja ataskaitą populiariausių `N` URL, jų kiekio.
* Srautas pagal valandą: sukurkite skriptą, kuris analizuoja `access_log` ir parengia ataskaitą, rodančią svetainės srautą pagal dienos valandas.
* Srautas pagal lankytoją: sukurkite skriptą, kuris apdoroja svetainės `access_log` failą ir skaičiuoja kiekvieno unikalaus lankytojo IP adreso suvartojamą srautą. Turėtų būti išvardyti N daugiausiai srauto suvartojęi IP adresai, jų suvartotas srautas.
* Užklausos metodų analizė: sukurkite skriptą, kuris analizuoja `access_log`, kad praneštų apie lankytojų naudojamų HTTP užklausų metodų (GET, POST ir kt.) pasiskirstymą.
* Vartotojų grupės: parašykite skriptą, kuris naudoja `/etc/passwd` ir išvardija grupes, kurioms priklauso nurodytas vartotojas.
* Išvardykite vartotojus su konkrečiu apvalkalu: sukurkite skriptą, kuris naudoja apvalkalo pavadinimą kaip argumentą (pvz: `/bin/bash`) ir išvardija visas naudotojų paskyras faile `/etc/passwd`, kurios naudoja tą apvalkalą.
* El. pašto adreso tikrinimo priemonė: sukurkite apvalkalo skriptą, kuris pagal įprastus el. pašto adresų šablonus patikrintų, ar įvesties eilutė yra galiojantis el. pašto adresas.
* URL tikrintuvas: parašykite skriptą, kuris patikrina, ar nurodyta įvesties eilutė yra tinkamas URL, užtikrinant, kad jis prasidėtų „http://“ arba „https://“.
* Slaptažodžio stiprumo tikrintuvas: sukurkite skriptą, kuris įvertina vartotojo įvesto slaptažodžio stiprumą pagal tokius kriterijus kaip ilgis, didžiosios raidės, skaičiai ir specialieji simboliai.
* Telefono numerio tikrinimo priemonė: sukurkite skriptą, patvirtinantį, ar įvesties eilutė yra galiojantis telefono numeris, atitinkantis nurodytą formatą (pvz., +370 600 12345).
* Failo kelio tikrinimo priemonė: parašykite skriptą, kuris patikrina, ar nurodyta įvesties eilutė atitinka galiojantį failo kelią ir egzistuoja failų sistemoje.
* Datos formato tikrintuvas: sukurkite skriptą, patvirtinantį, ar įvesties datos eilutė atitinka tam tikrą datos formatą (pvz., YYYY-MM-DD).
* IP adreso tikrintuvas: parašykite skriptą, kuris patikrina, ar įvesties eilutė yra tinkamas IPv4 arba IPv6 adresas, ir praneša apie adreso tipą.
* Domeno vardo tikrintuvas: sukurkite skriptą, kuris patikrina, ar nurodyta įvesties eilutė yra galiojantis domeno vardas pagal DNS pavadinimų suteikimo taisykles.
* Nuorodų rinkiklis: sukurkite skriptą, kuris iš duoto URL į HTML tinklalapį ištraukia visus hipersaitus (URL) ir pateikia jų sąrašą.
* Žodžių dažnio skaitiklis: parašykite skriptą, kuris iš duoto URL į HTML skaičiuoja žodžių, naudojamų tinklalapio teksto turinyje, dažnį ir rodo dažniausiai vartojamus žodžius.
* Metaduomenų ekstraktorius: sukurkite skriptą, kuris iš HTML `<meta>` žymų ištraukia metaduomenų informaciją, pvz., autorių, aprašymą ir raktinius žodžius.
* Konverteris iš lentelės į CSV: sukurkite skriptą, kuris analizuoja HTML lenteles ir konvertuoja jų turinį į CSV (kableliais atskirtų verčių) formatą.
* Paieškos raktinio žodžio paryškinimo priemonė: sukurkite skriptą, kuris naudoja paieškos raktinį žodį kaip įvestį ir paryškina to raktinio žodžio atvejus tinklalapio teksto turinyje.
* CSS ir JavaScript failų nuorodos: sukurkite skriptą, kuris ištraukia ir pateikia nuorodas į išorinius CSS ir JavaScript failus, naudojamus tinklalapyje.
* Turinio generatorius: sukurkite skriptą, kuris generuoja turinį pagal HTML dokumento antraštes (nuo `<h1>` iki `<h6>`), pateikdamas nuorodas į kiekvieną skyrių.
* Atributo vertės ištraukiklis: parašykite skriptą, kuris kaip įvestį paima HTML failą ir HTML žymą bei atributo pavadinimą, ištraukia ir pateikia visas atributų reikšmes nurodytu pavadinimu.
* Failo eilučių numeriai: sukurkite skriptą, kuris prideda eilučių numerius prie kiekvienos tekstinio failo eilutės ir sukuria naują failą su sunumeruotomis eilutėmis. Nenaudojate `cat`.
* Žodžių dažnio analizė: sukurkite skriptą, kuris analizuoja žodžių dažnį tekstiniame faile ir rodo dažniausiai vartojamų žodžių sąrašą.
* CSV failų keitiklis: sukurkite skriptą, kuris konvertuoja CSV failą į HTML, išsaugant duomenų struktūrą.
* CSV stulpelių statistika: parašykite skriptą, kuris apskaičiuoja pagrindinę statistiką (suma, vidurkis, didžiausias, minimumas) nurodytam N skaitiniam stulpeliui CSV faile.
* Pasikartojančių failų ieškiklis: sukurkite skriptą, kuris identifikuoja ir išvardija pasikartojančius failus kataloge pagal jų pavadinimą.
* Katalogų medis į HTML sąrašą: parašykite skriptą, kuris konvertuoja katalogų medžio struktūrą į HTML sąrašą, rodydamas katalogus ir failus kaip spustelėjamas nuorodas.
* Vaizdų galerijos generatorius: parašykite apvalkalo skriptą, kuris generuoja HTML vaizdų galeriją iš nurodyto katalogo, kuriame yra vaizdo failų.

