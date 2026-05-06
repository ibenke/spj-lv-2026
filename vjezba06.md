![Header VUV](/img/logo_header.png "Header VUV")

# 6. Laboratorijska vježba

## Sadržaj vježbe

* Zadaci za rad u laboratoriju
* Popis API ruta
---

## Zadaci za rad u laboratoriju

### Zadatak 1

Potrebno je kreirati novu React aplikaciju naredbom:

```bash
npm create vite@latest
```

Ime aplikacije treba biti:

```text
react-employees
```

Nakon toga potrebno je instalirati sljedeće pakete:

```bash
npm install bootstrap@5.3.3
npm install react-bootstrap
npm install react-router-dom
npm install axios
npm install react-datepicker
```

Paketi se koriste za:

* `bootstrap` – Bootstrap framework
* `react-bootstrap` – Bootstrap komponente za React
* `react-router-dom` – navigacija između stranica
* `axios` – komunikacija s API-jem
* `react-datepicker` – odabir datuma u React aplikaciji

---

### Zadatak 2

Nakon konfiguracije potrebno je kreirati sljedeće komponente:

```text
Navigacija.jsx
Pocetna.jsx
Uredi.jsx
Obrisi.jsx
Dodaj.jsx
```

Opis komponenti:

* `Navigacija.jsx` – navigacija između stranica **Početna** i **Dodaj**
* `Pocetna.jsx` – tablica sa prikazom zaposlenika
* `Uredi.jsx` – stranica koja sadrži formu za uređivanje zaposlenika
* `Obrisi.jsx` – stranica na kojoj se potvrđuje brisanje zaposlenika
* `Dodaj.jsx` – stranica koja sadrži formu za dodavanje zaposlenika

---

### Zadatak 3

Komponenta:

```text
Navigacija.jsx
```

treba sadržavati **navbar** sa dva linka:

* `Početna`
* `Dodaj`

---

### Zadatak 4

Komponenta:

```text
Pocetna.jsx
```

treba sadržavati **tablicu sa prikazom zaposlenika**.

Nije potrebno rastavljati prikaz na više komponenti kao u prethodnoj vježbi.

Na početnoj stranici prikazati popis zaposlenika dohvaćen s API-ja.

![Zadatak 4](/img/lv6_zadatak4.jpg "Početna stranica")

---

### Zadatak 5

Komponenta:

```text
Uredi.jsx
```

treba sadržavati **formu za uređivanje zaposlenika**.

Stranica se otvara klikom na gumb:

```text
Uredi
```

Potrebno je dohvatiti podatke odabranog zaposlenika i omogućiti njihovu izmjenu.

![Zadatak 5](/img/lv6_zadatak5.jpg "Uređivanje")

---

### Zadatak 6

Komponenta:

```text
Obrisi.jsx
```

treba sadržavati stranicu na kojoj se potvrđuje brisanje zaposlenika.

Stranica se otvara klikom na gumb:

```text
Obriši
```

Na ovoj stranici potrebno je potvrditi brisanje odabranog zaposlenika.

![Zadatak 6](/img/lv6_zadatak6.jpg "Brisanje")

---

### Zadatak 7

Komponenta:

```text
Dodaj.jsx
```

treba sadržavati **formu za dodavanje zaposlenika**.

Stranica se otvara klikom na link iz navigacije:

```text
Dodaj
```

Putem forme potrebno je omogućiti unos novog zaposlenika.

![Zadatak 7](/img/lv6_zadatak7.jpg "Dodavanje")
---

#### Popis potrebnih API ruta nalazi se na linku:

http://31.147.206.172:8083/swagger/index.html