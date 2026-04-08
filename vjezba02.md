![Header VUV](/img/logo_header.png "Header VUV")

# 2. Laboratorijska vježba

## Sadržaj vježbe

* Zadaci za rad u laboratoriju

---

## Zadaci za rad u laboratoriju

> [!NOTE]
> **Prije početka vježbe:**
>
> Preko terminala provjeriti je li **Node.js** instaliran:
>
> ```bash
> node -v
> ```
>
> Ako je **Node.js** ispravno instaliran, u terminalu će se ispisati njegova verzija.

### Zadatak 1

Koristeći **Node.js naredbeni redak**, kreirati mapu:

```text
D:\{Prezime_Ime}
```

Pozicionirati se u kreiranu mapu i u njoj kreirati novu mapu naziva:

```text
LV2
```

Pozicionirati se u mapu **LV2** i u njoj kreirati datoteku:

```text
server.js
```

---

### Zadatak 2

Pokrenuti program za pisanje koda (**VS Code**) i otvoriti mapu:

```text
{Prezime_Ime}
```
zatim u datoteku:

```text
server.js
```
Napisati program koji će:

* kreirati jednostavan **HTTP server**
* server treba raditi na portu:

```text
8008
```

Kreirati varijablu:

```javascript
sIme
```

U nju spremiti svoje **ime i prezime**.

Kao odgovor server treba poslati vrijednost zapisanu u varijabli `sIme`.

Pokretanje programa:

```bash
node server.js
```

---

### Zadatak 3

Kreirati novu datoteku:

```text
zadatak3.js
```

Napisati program koji će za **prvih 100 brojeva** provjeriti djeljivost prema sljedećim uvjetima:

* ukoliko je broj djeljiv sa **5**, ispisati poruku
  `"Broj {n} je djeljiv sa 5"`

* ukoliko je broj djeljiv sa **7**, ispisati poruku
  `"Broj {n} je djeljiv sa 7"`

* ukoliko je broj djeljiv i sa **5 i sa 7**, ispisati poruku
  `"Broj je djeljiv i sa 5 i sa 7"`

Program pokrenuti naredbom:

```bash
node zadatak3.js
```

---

### Zadatak 4

Kreirati novu datoteku:

```text
zadatak4.js
```

Napisati program koji će izračunati **sumu prvih 100 neparnih brojeva**.

Dobivenu sumu ispisati u konzolu.

Pokretanje:

```bash
node zadatak4.js
```

---

### Zadatak 5

Kreirati novu datoteku:

```text
zadatak5.js
```

Kreirati prazno polje:

```javascript
aPolje
```

Napisati program koji će u polje spremiti **prvih 50 brojeva djeljivih sa 7**.

Nakon toga kreirati novo polje:

```javascript
aParniBrojevi
```

U njega spremiti **sve parne brojeve iz polja `aPolje`**.

U konzolu ispisati sadržaj polja `aParniBrojevi`.

Pokretanje:

```bash
node zadatak5.js
```

---

### Zadatak 6

Kreirati novu datoteku:

```text
slucajanBroj.js
```

U nju upisati funkciju:

```javascript
function dajSlucajanBroj(nMin, nMax)
{
    return Math.floor(Math.random() * (nMax - nMin + 1) + nMin);
}
```

Kreirati novu datoteku:

```text
zadatak6.js
```

Napisati program koji će:

* generirati **100 slučajnih brojeva**
* raspon brojeva: **50 – 5000**
* brojeve spremiti u polje `aBrojevi`

Potrebno je ispisati:

* koliko je **parnih brojeva**
* koliko je **neparnih brojeva**

Pokretanje:

```bash
node zadatak6.js
```

---

### Zadatak 7

Kreirati datoteku:

```text
zadatak7.js
```

Koristeći funkciju za generiranje slučajnog broja:

* generirati **200 slučajnih brojeva**
* raspon: **150 – 1500**

Brojeve spremiti u polje `aBrojevi`.

Potrebno je ispisati:

* **najmanji broj**
* **najveći broj**

Pokretanje:

```bash
node zadatak7.js
```

---

### Zadatak 8

Kreirati datoteku:

```text
zadatak8.js
```

Koristeći funkciju za generiranje slučajnog broja:

* generirati **50 slučajnih brojeva**
* raspon: **1 – 20**

Brojeve spremiti u polje `aBrojevi`.

Potrebno je ispisati **jedinstvene brojeve polja (bez ponavljanja)**.

Prije rješavanja zadatka proučiti funkciju:

```text
indexOf()
```

Dokumentacija:

```text
https://www.w3schools.com/jsref/jsref_indexof_array.asp
```

---

### Zadatak 9

Zadana su dva polja:

```javascript
var aPolje1 = [1, 4, 7, 8, 9, 12, 16, 18, 22, 24, 25];
var aPolje2 = [2, 3, 4, 7, 8, 11, 13, 15, 17, 18, 22, 23];
```

Kreirati datoteku:

```text
zadatak9.js
```

Napisati program koji će ispisati **brojeve koji su zajednički poljima** `aPolje1` i `aPolje2`.

Prije rješavanja zadatka proučiti funkciju:

```text
indexOf()
```

Dokumentacija:

```text
https://www.w3schools.com/jsref/jsref_indexof_array.asp
```

---

### Zadatak 10

Kreirati datoteku:

```text
zadatak10.js
```

Napisati program koji će kreirati **HTTP server** na portu:

```text
8000
```

Server treba u preglednik ispisati **10 slučajnih brojeva** u rasponu:

```text
10 – 100
```

Odgovor treba biti tipa **String**, stoga je potrebno broj pretvoriti pomoću funkcije:

```javascript
String(nBroj) + "\n"
```

Otvoriti u pregledniku:

```text
http://localhost:8000
```

---

### Zadatak 11

Kreirati datoteke:

```text
zadatak11.js
osobe.json
```

Datoteka `osobe.json` treba sadržavati podatke o osobama:

```json
[
  {
    "index": 0,
    "age": 39,
    "name": "Marko Marić",
    "company": "BEDDER"
  },
  {
    "index": 1,
    "age": 31,
    "name": "Ivan Horvat",
    "company": "FLOTONIC"
  },
  {
    "index": 2,
    "age": 34,
    "name": "Petar Filipović",
    "company": "ENJOLA"
  },
  {
    "index": 3,
    "age": 37,
    "name": "Ana Novak"
  },
  {
    "index": 4,
    "age": 35,
    "name": "Marta Perić",
    "company": "RADIANTIX"
  }
]
```

Potrebno je:

* kreirati **HTTP server**
* pročitati podatke iz datoteke `osobe.json`
* ispisati ih u web pregledniku

Koristiti Node.js module:

* `http`
* `fs`

Otvoriti u pregledniku:

```text
http://localhost:8000
```

---

### Zadatak 12

Kreirati tri datoteke:

```text
broker.js
publisher.js
subscriber.js
```

Koristiti predložak iz predavanja koji opisuje upotrebu **MQTT modula**.

Publisher treba:

* generirati slučajne brojeve
* raspon **10 – 1000**
* poslati ih subscriberu

Subscriber treba:

* primiti brojeve
* spremiti ih u **tekstualnu datoteku**

Potrebno je instalirati module:

```bash
npm install mqtt
npm install mosca
```

---

### Zadatak 13

Kreirati datoteku:

```text
zadatak13.js
```

Koristeći funkciju za generiranje slučajnog broja:

* generirati **30 slučajnih brojeva**
* raspon **10 – 200**

Brojeve spremiti u polje `aBrojevi`.

Napisati program koji će **sortirati polje bez korištenja metode `sort()`**.

---

### Zadatak 14

Kreirati datoteku:

```text
zadatak14.js
```

Napisati program koji će:

* ispisati **zbroj prve i zadnje znamenke broja**
* provjeriti da je uneseni broj **veći od 99**

---

### Zadatak 15

Kreirati datoteku:

```text
zadatak15.js
```

Koristeći funkciju za generiranje slučajnog broja:

* generirati **tri slučajna broja**
* raspon **10 – 100**

Usporediti **zadnje znamenke brojeva**.

Ispisati:

```text
true
```

ako se zadnja znamenka podudara u **najmanje dva broja**.

Primjer:

```text
34, 56, 66 -> true
```

jer se zadnje znamenke **56 i 66 podudaraju**.

---