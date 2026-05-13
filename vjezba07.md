![Header VUV](/img/logo_header.png "Header VUV")

# 7. Laboratorijska vježba

## Sadržaj vježbe

* Zadaci za rad u laboratoriju

---

## Zadaci za rad u laboratoriju

### Zadatak 1

Potrebno je kreirati Vue aplikaciju naredbom:

```bash
npm create vite@latest
```

Naziv projekta treba biti:

```text
trgovina_vue_prezime
```

`prezime` zamijeniti vlastitim prezimenom.

Nakon kreiranja projekta:

* u mapi `components` obrisati datoteku:

```text
HelloWorld.vue
```

Datoteku:

```text
App.vue
```

promatrati kao **vršnu (roditeljsku) komponentu**.

Njezin sadržaj zamijeniti sljedećim predloškom:

```vue
<script setup>
</script>

<template>
</template>

<style scoped>
</style>
```

---

### Zadatak 2

Kreirati JSON datoteku:

```text
artikli.json
```

Svaki objekt (artikl) treba sadržavati sljedeća svojstva:

* `id`
* `naziv`
* `opis`
* `cijena`
* `kolicina`

Potrebno je dodati nekoliko artikala.

---

### Zadatak 3

Za stiliziranje koristiti **Bootstrap**.

Prije pokretanja naredbe potrebno je pozicionirati se u mapu aplikacije.

Pokrenuti naredbu:

```bash
npm install bootstrap@5.3.3
```

Nakon instalacije potrebno je u datoteci:

```text
main.js
```

dodati linije:

```javascript
import 'bootstrap/dist/css/bootstrap.min.css';
import 'bootstrap/dist/js/bootstrap.bundle.js';
```

te obrisati liniju:

```javascript
import './style.css'
```

---

### Zadatak 4

U mapu:

```text
components
```

potrebno je dodati tri nove komponente:

* `Zaglavlje.vue`
* `TrgovinaArtikl.vue`
* `TrgovinaLista.vue`

Opis komponenti:

**Zaglavlje.vue**

Komponenta sadrži **navbar** sa logom i nazivom trgovine.

---

**TrgovinaArtikl.vue**

Komponenta predstavlja **jedan artikl u tablici**, odnosno jedan redak:

```html
<tr>
```

---

**TrgovinaLista.vue**

Komponenta predstavlja **tablicu sa svim artiklima**, odnosno:

```html
<table>
```

---

### Zadatak 5

Vratiti se u komponentu:

```text
App.vue
```

Potrebno je napraviti **import prethodno kreiranih komponenti**:

* `Zaglavlje.vue`
* `TrgovinaLista.vue`

Osim toga potrebno je napraviti i **import podataka iz datoteke**:

```text
artikli.json
```

Nakon importa i poziva komponenti na stranici bi trebalo biti vidljivo:

* zaglavlje
* tablica sa podacima

---

### Zadatak 6

Unutar komponente:

```text
TrgovinaArtikl.vue
```

potrebno je dodati gumb koji se prikazuje ovisno o količini artikla.

##### Uvjet 1

Ako je količina artikla veća od:

```text
0
```

prikazuje se gumb sa tekstom:

```text
Dodaj
```

Klikom na gumb potrebno je prikazati poruku:

```text
Artikl {imeArtikla} je dodan u košaricu.
```

---

##### Uvjet 2

Ako je količina artikla jednaka:

```text
0
```

prikazuje se gumb sa tekstom:

```text
Pošalji upit
```

Klikom na gumb potrebno je prikazati poruku:

```text
Upit za {imeArtikla} je poslan.
```

---