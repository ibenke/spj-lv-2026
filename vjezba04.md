![Header VUV](/img/logo_header.png "Header VUV")

# 4. Laboratorijska vježba

## Sadržaj vježbe

* Zadaci za rad u laboratoriju

---

## Zadaci za rad u laboratoriju

Prije početka rješavanja zadataka potrebno je s loomen stranice kolegija preuzeti predložak sa strukturom datoteka i mapa **prilog_lv4.rar.**

Vježba se sastoji od **8 obaveznih zadataka** u kojima studenti imaju slobodu odabira tehnologije:

* JavaScript
* jQuery

Unutar mape koja je kreirana na prvoj vježbi, a nalazi se na:

```text
D:\{Prezime_Ime}
```

Potrebno je kreirati novu mapu:

```text
LV4
```

Strukturu `prilog_lv4` preuzetu s loomena dodati u mapu `LV4`.

---

### Zadatak 1 – To-Do lista

Napisati JavaScript/jQuery aplikaciju koja služi korisnicima za zapisivanje zadataka.

U datoteci:

```text
to-do-list.html
```

potrebno je napraviti kostur aplikacije koji treba sadržavati element:

```html
<ul>
```

unutar kojega će se nalaziti lista zadataka.

Aplikacija treba omogućiti korisniku da:

* unese naziv zadatka unutar tekstualnog okvira
* klikom na gumbić **Dodaj** prikaže zadatak u listi

Akcije u listi trebaju omogućiti:

* promjenu statusa zadatka
* brisanje elementa sa liste

Za ikone koristiti:

```text
font-awesome
```

![Zadatak 1](/img/lv4_zadatak1.jpg "To do lista")

---

### Zadatak 2 – Dinamična galerija slika

Kreirati dinamičnu galeriju slika sa slikama koje se nalaze u mapi:

```text
img
```

Zadan je HTML dokument:

```text
slider.html
```

sa kosturom, a potrebno je u datoteci:

```text
slider.js
```

napisati kod koji će HTML dokumentu dodati dinamičan pregled slika pomoću gumbića.

![Zadatak 2](/img/lv4_zadatak2.jpg "Galerija slika")

---

### Zadatak 3 – Forma

Zadana je datoteka:

```text
forma.html
```

koja sadrži obrazac.

U obrascu se nalaze sljedeća polja za popunjavanje:

* Ime studenta
* Prezime studenta
* JMBAG
* OIB
* Datum rođenja
* Adresa
* Poštanski broj
* Grad

Potrebno je u datoteci:

```text
forma.js
```

napisati kod koji će klikom na gumbić **Spremi** provjeriti jesu li sva polja obrasca popunjena.

Ako su sva polja popunjena, potrebno je kreirati objekt koji sadrži upisane podatke.

U suprotnom je potrebno ispisati poruku u malom prozoru da nisu popunjena sva polja.

Datum rođenja se u `input` element upisuje u formatu:

```text
09-06-2006
```

Potrebno je provjeriti je li format datuma točan. Ako nije, prikazati poruku.

Ako je datum rođenja točno zapisan, prije pohranjivanja u objekt potrebno je promijeniti format u:

```text
2006-06-09
```

Polja za:

* JMBAG
* OIB
* poštanski broj

trebaju sadržavati samo brojeve, primjerice uz pomoć:

```text
regex
```

Nakon uspješnog kreiranja objekta, ispisati ga u konzoli pomoću funkcije:

```javascript
console.log()
```

> [!NOTE]
> Prije obrade forme potrebno je spriječiti zadano ponašanje:
>
> ```javascript
> event.preventDefault();
> ```


![Zadatak 3](/img/lv4_zadatak3.jpg "Podaci student")

---

### Zadatak 4 – Boje

Kreirati datoteku:

```text
boje.js
```

u kojoj treba napisati funkciju za slučajni odabir boja.

Koristiti:

* predefinirane boje, npr. `yellow`, `green`, `orangered`
* heksadecimalne boje
* RGB boje

> [!NOTE]
> Preporučuje se implementirati funkcije:
>
> ```javascript
> function getHexa() //#f4f4f4
> function getRgb() //rgb(245, 230, 72)
> function getPredefined() //yellow
> ```
>
> i glavnu funkciju:
>
> ```javascript
> function getColor()
> ```
>
> Funkcija `getColor()`:
>
> * odabire jednu od tri funkcije
> * prikazuje vrijednost boje
> * postavlja boju pozadine


Klikom na gumb potrebno je:

* generirati boju
* postaviti tu boju kao `background` boju stranice
* ime boje ispisati u `h2` elementu

U datoteci:

```text
boje.html
```

trebaju se nalaziti samo:

* gumb
* element za ispis imena boje

Potrebno ih je centrirati na sredinu stranice.

![Zadatak 4](/img/lv4_zadatak4.jpg "Promjena boje")

---

### Zadatak 5 – Konverter valuta

Kreirati novu datoteku:

```text
konvert.js
```

Napisati konverter valuta za najmanje **5 valuta**.

Konverziju treba omogućiti:

* iz svake valute u svaku valutu

> [!NOTE]
> Ovaj objekt sadrži tečajeve konverzije između valuta koje je potrebno dohvatiti i primijeniti pri izračunu.
>
> ```javascript
> var tecaj = {
>     USD: { EUR: 0.85, GBP: 0.72, JPY: 113.54, AUD: 1.32 },
>     EUR: { USD: 1.07, GBP: 0.86, JPY: 133.89, AUD: 1.55 },
>     GBP: { USD: 1.39, EUR: 1.18, JPY: 157.04, AUD: 1.82 },
>     JPY: { USD: 0.0088, EUR: 0.0075, GBP: 0.0064, AUD: 0.012 },
>     AUD: { USD: 0.76, EUR: 0.65, GBP: 0.55, JPY: 83.75 }
> };
> ```

U datoteci:

```text
konvert.html
```

koristiti:

* padajuće izbornike za odabir valute
* `input` element za upis vrijednosti za konverziju

![Zadatak 5](/img/lv4_zadatak5.jpg "Konverter")

---

### Zadatak 6 – Lista literature

Kreirati novu datoteku:

```text
lista.js
```

Napraviti listu literature po predmetima koju je moguće:

* sakriti
* prikazati

Klikom na link pojedine literature, na desnoj strani treba prikazati sliku navedene literature.

![Zadatak 6](/img/lv4_zadatak6.jpg "Literatura")

---

### Zadatak 7 – Sortiranje liste

Kreirati datoteku:

```text
sort.js
```

Napraviti listu u kojoj je uz pomoć miša moguće sortirati elemente.

![Zadatak 7](/img/lv4_zadatak7.jpg "Sortiranje")

---

### Zadatak 8 – Atributi input elementa

Kreirati datoteku:

```text
atributi.js
```

Na stranicu:

```text
atributi.html
```

potrebno je postaviti padajući izbornik koji služi za odabir tipa podataka:

* `email`
* `number`
* `password`
* `text`

Odabrani tip podatka treba biti postavljen kao tip podatka kod novo kreiranog `input` elementa.

Potrebno je kreirati i gumb koji će vrijednost unesenu u `input` element spremiti u:

```text
json datoteku
```
![Zadatak 8](/img/lv4_zadatak8.jpg "Input element")

---