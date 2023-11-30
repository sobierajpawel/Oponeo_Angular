# Dyrektywy

1. Utwórz nową dyrektywę w angularze

```
ng g directive <nazwa-dyrektywy> --skip-tests
```

2. Napisz dyrektywę, która przyjmuje przynajmniej jeden parametr zewnętrzny za pomocą słowa kluczowego `@Input`.
3. Dyrektywa powinna działać na zdarzenie lub wiele zdarzeń (np. `mouseleave`, `mouseenter`). Wykorzystaj dekorator `@HostListener` do obsługi tych zdarzeń.
4. Napisz dekorator, który zmienia tło, zmienia czcionkę (może również zapisywać stan stylu orginalnego tak by powrócić do oryginalnej formy).

----------------------------------------------------------------------------------------------------------------------
en

# Directives
1. Create a new directive in Angular
```
ng g directive <nazwa-dyrektywy> --skip-tests
```
2. Write a directive that takes at least one external parameter using the @Input keyword.
3. The directive should act on an event or multiple events (e.g. mouseleave, mouseenter). Use the @HostListener decorator to handle these events.
4. Write a decorator that changes the background, changes the font (it can also save the state of the original style so it can return to its original form).
