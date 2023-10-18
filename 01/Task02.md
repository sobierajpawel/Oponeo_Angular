# Zmiana struktury projektu oraz dodanie Bootstrap'a

1. Usuń z pliku app.component.html zawartość między komentarzami.

2. Wprowadź zmiany w kodzie html.

```html
<header class="container">
  <h1>
    {{ title }}
  </h1>
</header>

<main class="container">
  <router-outlet></router-outlet>
</main>

<footer class="container">
</footer>
```

3. Wprowadź zmiany w komponencie do zmiennej `title`. Dodaj zmienną `footer` i osadź ją w komponencie html w stopce. Uruchom aplikacje i zobacz zmiany w przeglądarce.

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  title = 'Aplikacja zarządzająca studentami';
  footer = "Copyright 2023 by SDA.";
}

```

```html
<header class="container">
  <h1>
    {{ title }}
  </h1>
</header>

<main class="container">
  <router-outlet></router-outlet>
</main>

<footer class="container">
{{ footer }}
</footer>
```


4. Zainstaluj bootstrap w projekcie poleceniem za pomocą menadżera pakietów NPM.

```ps
  npm install bootstrap --save
```

5. Dodaj następujące skrypty dla css oraz js w pliku `angular.json`.

```json
    "styles": 
    [
      "node_modules/bootstrap/dist/css/bootstrap.min.css",
      "src/styles.css"
     ],
     "scripts": 
     [
      "./node_modules/bootstrap/dist/js/bootstrap.js"
     ]
```


6. Przetestuj czy bootstrap działa prawidłowo - np. czy widzisz przycisk z bootstrapa.

7. Dodaj nawigację do projektu - może to być navbar z bootstrapa. Dostosuj główny layout swojej aplikacji. Możesz dodać stopkę.

8. Postaraj się odseparować nawigację oraz stopkę do osobnego komponentu.
```
ng g component `nazwa-komponentu`
```
