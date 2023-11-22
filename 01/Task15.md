# Własny kontener toastów i komunikacja między komponentami z wykorzystaniem RxJS

1. Zbuduj własny komponent toastu - możesz bazować na

```html
<div class="toast show align-items-center text-white bg-primary border-0" 
    style="margin-top:10px"
    role="alert" aria-live="assertive"
    aria-atomic="true">
    <div class="d-flex">
      <div class="toast-body">
        Tekst toasta
      </div>
      <button type="button" class="btn-close btn-close-white me-2 m-auto" data-bs-dismiss="toast"
        aria-label="Close"></button>
    </div>
  </div>
```

2. Wykorzystaj nowy serwis, który skorzysta z obiektu `Subject` do którego może podpiać się wielu subskrybentów.

```ts
  private toastsSubject = new Subject<string>();
```

3. Osadź wyświetlanie toastów w określonym miejscu w twojej aplikacji (na dole po prawej, lewej lub na środku ekranu), umożliw wyświetlanie wielu toastów na raz. Postaraj sie je schować po jakimś czasie.

4. Zbuduj mechanizm, który umożliwi wyświetlanie toastów w różnych kolorach zależnie od błędu, sukcesu.

5. Przebuduj aplikację w taki sposób aby wykorzystywała ona toasty we wszystkich przypadkach zamiast obecnie używanych mechanizmów.
