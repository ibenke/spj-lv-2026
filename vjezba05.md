![Header VUV](/img/logo_header.png "Header VUV")

# 5. Laboratorijska vježba

## Sadržaj vježbe

* Zadaci za rad u laboratoriju

---

## Zadaci za rad u laboratoriju

### Zadatak 1

Potrebno je kreirati novu React aplikaciju naredbom:

```bash
npm create vite@latest
```

Nakon pokretanja naredbe:

* za **project name** upisati:

```text
trgovina-prezime
```

`prezime` zamijeniti vlastitim prezimenom.

* za **Select a framework** odabrati:

```text
React
```

* za **Select a variant** odabrati:

```text
JavaScript
```

![Zadatak 1](/img/lv5_zadatak1a.jpg "Kreiranje projekta")

Nakon toga pokrenuti sljedeće naredbe:

```bash
cd trgovina-prezime
npm install
npm run dev
```

Otvoriti aplikaciju u **Visual Studio Codeu**.

![Zadatak 1](/img/lv5_zadatak1b.jpg "Struktura react aplikacije")

U mapi:

```text
src
```

nalazi se datoteka:

```text
App.jsx
```

Tu datoteku promatrati kao vršnu odnosno roditeljsku komponentu.

Njezin sadržaj zamijeniti sljedećim predloškom:

```javascript
function App() {
  return (
    <>
    </>
  );
}

export default App;
```

---

### Zadatak 2

Unutar mape:

```text
assets
```

kreirati JSON datoteku:

```text
artikli.json
```

Svaki objekt, odnosno artikl, treba sadržavati sljedeća svojstva:

* `id`
* `naziv`
* `opis`
* `cijena`
* `kolicina`

Potrebno je dodati najmanje **5 artikala** iz područja:

```text
IT oprema
```

---

### Zadatak 3

Za stiliziranje koristiti:

```text
Bootstrap
```

Bootstrap je potrebno uključiti instalacijom paketa.

Prije pokretanja naredbe potrebno se pozicionirati u mapu aplikacije.

Pokrenuti naredbu:

```bash
npm install bootstrap@5.3.3
```

Nakon toga u datoteci:

```text
main.jsx
```

dodati liniju:

```javascript
import 'bootstrap/dist/css/bootstrap.min.css';
```

i maknuti liniju:

```javascript
import './index.css';
```

---

### Zadatak 4

U mapu:

```text
src
```

potrebno je dodati tri nove komponente:

```text
Zaglavlje.jsx
TrgovinaArtikl.jsx
TrgovinaTablica.jsx
```

##### Zaglavlje.jsx

Ova komponenta treba sadržavati **navbar**.

Koristiti Bootstrap dokumentaciju, dio:

```text
navbar -> Image and text
```

Za sliku (logo) iskoristiti datoteku:

```text
react.svg
```

koja se nalazi u mapi `assets`.
Logo dodati kao props `logo`
Za tekst upisati:

```text
Trgovina {Prezime}
```

---

##### TrgovinaArtikl.jsx

Ova komponenta treba sadržavati definiciju za jedan redak u tablici:

```html
<tr>
```

Jedan redak predstavlja jedan artikl.

---

##### TrgovinaTablica.jsx

Ova komponenta treba sadržavati definiciju za tablicu:

```html
<table>
```

Potrebno je napraviti import komponente:

```text
TrgovinaArtikl
```

i uključiti ju u tablicu.

---

### Zadatak 5

Vratiti se u komponentu:

```text
App.jsx
```

Potrebno je napraviti import prethodno kreiranih komponenti:

* `Zaglavlje`
* `TrgovinaTablica`

Osim toga, potrebno je napraviti i import artikala iz datoteke:

```text
artikli.json
```

Nakon importa i poziva komponenti, na stranici bi trebalo biti vidljivo:

* zaglavlje
* tablica sa podacima

---

### Zadatak 6

Unutar datoteke:

```text
TrgovinaArtikl.jsx
```

potrebno je dodati komponentu **Gumb** koja se renderira u svakom retku (za svaki artikl) ovisno o uvjetu.

##### Uvjet 1

Ako je količina pojedinog artikla veća od:

```text
0
```

prikazuje se gumb s tekstom:

```text
Dodaj
```

Klikom na gumb pojavljuje se poruka:

```text
Artikl {imeArtikla} je dodan u košaricu.
```

---

##### Uvjet 2

Ako je količina artikla jednaka:

```text
0
```

prikazuje se gumb s tekstom:

```text
Pošalji upit
```

Klikom na gumb pojavljuje se poruka:

```text
Upit za {imeArtikla} je poslan.
```

![Zadatak 6](/img/lv5_zadatak6.jpg "Izgled aplikacije")
---