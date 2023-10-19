# Dodanie Bootstrapa

1. Usuń z pliku app.component.html zawartość między komentarzami.

2. Zainstaluj bootstrap w projekcie poleceniem za pomocą menadżera pakietów NPM.

```ps
  npm install bootstrap --save
```

3. Dodaj następujące skrypty dla css oraz js w pliku `angular.json`.

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


4. Przetestuj czy bootstrap działa prawidłowo - np. czy widzisz przycisk z bootstrapa.

