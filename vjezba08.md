![Header VUV](/img/logo_header.png "Header VUV")

# 8. Laboratorijska vježba

## Sadržaj vježbe

* Zadaci za rad u laboratoriju
* Popis API ruta

---

## Zadaci za rad u laboratoriju

### Zadatak 1

Potrebno je kreirati novu Vue aplikaciju naredbom:

```bash
npm create vite@latest
```

Ime aplikacije treba biti:

```text
vue-employees
```

Nakon toga potrebno je instalirati sljedeće pakete:

```bash
npm install bootstrap@5.3.3
npm install vue-router@4
npm install axios
npm install @vuepic/vue-datepicker
```

Paketi se koriste za:

* `bootstrap` – Bootstrap framework
* `vue-router` – navigacija između stranica
* `axios` – komunikacija s API-jem
* `@vuepic/vue-datepicker` – datepicker komponenta za Vue

---

### Zadatak 2

Nakon konfiguracije potrebno je kreirati sljedeće komponente:

* `Navigacija.vue`
* `Pocetna.vue`
* `Uredi.vue`
* `Obrisi.vue`
* `Dodaj.vue`

Opis komponenti:

* **Navigacija.vue** – navigacija između stranica **Početna** i **Dodaj**
* **Pocetna.vue** – tablica sa prikazom zaposlenika
* **Uredi.vue** – stranica koja sadrži formu za uređivanje zaposlenika
* **Obrisi.vue** – stranica na kojoj se potvrđuje brisanje zaposlenika
* **Dodaj.vue** – stranica koja sadrži formu za dodavanje zaposlenika

---

### Zadatak 3

Komponenta:

```text
Navigacija.vue
```

treba sadržavati **navbar** sa dva linka:

* `Početna`
* `Dodaj`

---

### Zadatak 4

Komponenta:

```text
Pocetna.vue
```

treba sadržavati **tablicu sa prikazom zaposlenika**.

Nije potrebno rastavljati prikaz na više komponenti kao u prethodnoj vježbi.

Na početnoj stranici potrebno je prikazati popis zaposlenika dohvaćen s API-ja.

Primjer izgleda stranice:

![Zadatak 4](/img/lv6_zadatak4.jpg "Početna stranica")

---

### Zadatak 5

Komponenta:

```text
Uredi.vue
```

treba sadržavati **formu za uređivanje zaposlenika**.

Stranica se otvara klikom na gumb:

```text
Uredi
```

Potrebno je dohvatiti podatke odabranog zaposlenika i omogućiti njihovu izmjenu.

Primjer izgleda stranice:

![Zadatak 5](/img/lv6_zadatak5.jpg "Uređivanje zaposlenika")

---

### Zadatak 6

Komponenta:

```text
Obrisi.vue
```

treba sadržavati stranicu na kojoj se potvrđuje brisanje zaposlenika.

Stranica se otvara klikom na gumb:

```text
Obriši
```

Na ovoj stranici potrebno je potvrditi brisanje odabranog zaposlenika.

Primjer izgleda stranice:

![Zadatak 6](/img/lv6_zadatak6.jpg "Brisanje zaposlenika")

---

### Zadatak 7

Komponenta:

```text
Dodaj.vue
```

treba sadržavati **formu za dodavanje zaposlenika**.

Stranica se otvara klikom na link iz navigacije:

```text
Dodaj
```

Putem forme potrebno je omogućiti unos novog zaposlenika.

Primjer izgleda stranice:

![Zadatak 7](/img/lv6_zadatak7.jpg "Dodavanje zaposlenika")

---

## Popis API ruta

#### Popis potrebnih API ruta nalazi se na linku:

http://31.147.206.172:8083/swagger/index.html