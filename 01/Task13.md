# Formularz reaktywny dla edycji zadań dla użytkownika

1. Dodaj przycisk w liście użytkowników do podglądu aktualnych zadań do zrobienia dla danego usera.

2. Stwórz nowy widok prezentujący dane w formie listy zadań tylko dla aktualnego użytkownika.

3. Dodaj możliwość filtrowania - wyświetlanie zadań zakończonych (completed = true), niezakończonych (completed = false),
wszystkich zadań niezależnie od statusu.

4. Zbuduj formularz reaktywny do aktualizacji nowego rekordu dla obiektu zadania do realizacji `Todo` (pola tytuł - input typu text, czy zakończone zadanie - checkbox, user id - select z wyborem użytkownika). 

6. Wykorzystaj wbudowane walidatory required, maxlength, minlength na polach.

7. Wyświetl błędy walidacji wraz ze szczegółem jaki błąd wystąpił.

8. Zapewnij by formularz nie będzie submitowany w momencie kiedy walidacja nie została spełniona.

9. Napisz serwis oraz żądanie PUT wysyłające nowe zadanie do realizacji pod adres url endpointu.
`https://jsonplaceholder.typicode.com/todos`
