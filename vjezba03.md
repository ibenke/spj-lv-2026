![Header VUV](/img/logo_header.png "Header VUV")

# 3. Laboratorijska vježba

## Sadržaj vježbe

* Zadaci za rad u laboratoriju

---

Unutar mape koja je kreirana na prošloj vježbi, a nalazi se na:

```text
D:\{Prezime_Ime}
```

Potrebno je kreirati novu mapu:

```text
LV3
```

Sve `datoteke` i `mape` koje se spominju u narednim zadacima potrebno je dodati u mapu `LV3`.

---

## Zadaci za rad u laboratoriju

### Zadatak 1 – Funkcija kao klasa (1)

U datoteci:

```text
grad.js
```

kreirati JavaScript funkciju naziva **Grad**, koja će služiti kao klasa na temelju koje će se kreirati objekti.

Funkcija prima 4 parametra:

* naziv grada
* broj stanovnika
* latituda
* longituda

Unutar djelokruga funkcije potrebno je kreirati 4 podatkovna člana u koje će se spremiti vrijednosti prenesene preko parametara.

Podatkovne članove spremiti koristeći sintaksu:

```javascript
this.naziv_clana = vrijednost_clana;
```

Kreirati 5 objekata funkcije `Grad` sa stvarnim podacima za gradove:

* Virovitica
* Koprivnica
* Bjelovar
* Osijek
* Zagreb

Objekte kreirati prema primjeru:

```javascript
var oNazivGrada = new Grad(parametar1, parametar2, parametar3, parametar4);
```

Stvarne podatke za pojedini grad potrebno je potražiti na internetu.

---

### Zadatak 2 – Funkcija kao klasa (2)

Za funkciju odnosno objekt `Grad` kreirati prototip funkciju:

```javascript
dajVelicinuGrada()
```

Funkcija treba vratiti identifikator veličine grada prema sljedećem pravilu:

* `1` – ukoliko grad ima manje od **30 000** stanovnika
* `2` – ukoliko grad ima više od **30 000** stanovnika i manje od **200 000** stanovnika
* `3` – ukoliko grad ima više od **200 000** stanovnika

---

### Zadatak 3 – Funkcija kao klasa (3)

Kreirati funkciju:

```javascript
dajUdaljenost()
```

Funkcija prima 2 parametra, odnosno 2 grada, i treba za proslijeđene gradove vratiti **zračnu udaljenost u kilometrima**.

> [!NOTE]
> Za izračun udaljenosti koristiti **Haversineovu formulu:**
>
> Primjer:
>
> ```bash
> https://stackoverflow.com/questions/14560999/using-the-haversine-formula-in-javascript
> ```

---

### Zadatak 4 – DOM biblioteka (1)

U mapi:

```text
js
```

kreirati datoteku:

```text
lib.js
```

U njoj kreirati klasu odnosno funkciju:

```javascript
_lib
```

koja će služiti kao biblioteka za upravljanje elementima na stranici.

Biblioteka bi trebala služiti kao zamjena za **jQuery**, s osnovnim radnjama nad HTML elementima.

Funkcija treba primati jedan parametar koji predstavlja **selektor elementa**.

Za početak, unutar klase potrebno je kreirati dva podatkovna člana:

* `selektor` – sadrži naziv selektora kao string
* `el` – sadrži objekt selektiranog elementa koristeći metodu `querySelectorAll()`

U mapi `js` kreirati i datoteku:

```text
mojaSkripta.js
```

Ona služi programeru za kreiranje objekata i pozivanje metoda iz biblioteke `_lib`.

Biblioteku testirati tako da se kreira objekt `_lib` sa proizvoljnim elementom sa stranice `index.html` i ispiše njegova vrijednost u konzolu.

---

### Zadatak 5 – DOM biblioteka (2)

Klasi `_lib` dodati prototip funkciju:

```javascript
ubaciElement()
```

Funkcija kao parametar prima objekt sa svojstvima:

* `naziv` – predstavlja naziv novog elementa
* `klasa` – elementu dodjeljuje CSS klasu
* `identifikator` – elementu dodjeljuje identifikator
* `tekst` – u tijelo elementa upisuje tekst

Svojstvo `naziv` je obavezno.

Ostala svojstva su opcionalna. Ukoliko nisu navedena, odnosno ako im je vrijednost prazan string, program ne bi trebao izvršiti kod za dodavanje tih atributa.

Funkcija `ubaciElement()` treba ubaciti kreirani element unutar objekta odnosno HTML elementa nad kojim je pozvana.

---

### Zadatak 6 – DOM biblioteka (3)

Klasi `_lib` dodati prototip funkcije:

* `dodajKlasu()` – odabranom elementu ili elementima dodaje naziv klase prenesen parametrom
* `dodajAtribut()` – odabranom elementu ili elementima dodaje naziv i vrijednost atributa
* `prikazi()` – odabrani element ili elemente prikazuje
* `sakrij()` – odabrani element ili elemente sakriva

Za prikaz i sakrivanje elemenata koristiti CSS svojstvo:

```css
visibility
```

---

### Zadatak 7 – DOM biblioteka (4)

Unutar objekta `localStorage` spremiti sljedeće poveznice:

```text
stem -> https://stem.vuv.hr/
loomen -> https://fakulteti.loomen.carnet.hr
studentski_dom -> http://studom.vsmti.hr/
office365 -> https://outlook.office365.com/owa/?realm=vuv.hr#path=/mail
```

Koristeći kreiranu DOM biblioteku, u podnožje stranice, unutar liste sa klasom:

```text
footernavigation
```

dodati poveznice spremljene unutar objekta `localStorage`.

Napomena:

* dodati element liste sa klasom `item`
* unutar njega dodati poveznicu, odnosno `<a>` element sa pripadajućim atributom poveznice

Za pristup pojedinom članu liste koristiti selektor:

```css
.item:nth-child(redni_broj_elementa)
```

Za pristup pojedinoj poveznici člana liste koristiti selektor:

```css
.item:nth-child(redni_broj_elementa) a
```

---