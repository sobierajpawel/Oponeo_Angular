# Dyrektywy

1. Utwórz nową dyrektywę w angularze

```
ng g directive <nazwa-dyrektywy> --skip-tests
```

2. Napisz dyrektywę, która przyjmuje przynajmniej jeden parametr zewnętrzny za pomocą słowa kluczowego `@Input`.
3. Dyrektywa powinna działać na zdarzenie lub wiele zdarzeń (np. `mouseleave`, `mouseenter`). Wykorzystaj dekorator `@HostListener` do obsługi tych zdarzeń.
4. Napisz dekorator, który zmienia tło, zmienia czcionkę (może również zapisywać stan stylu orginalnego tak by powrócić do oryginalnej formy). 
