# Formularz reaktywny dla edycji zadań dla użytkownika

1. W szczegółach użytkownika dodaj możliwość filtrowania - wyświetlanie zadań zakończonych (completed = true), niezakończonych (completed = false), wszystkich zadań niezależnie od statusu.

2. Po kliknięciu na dane zadanie powinno przejść ono do możliwości edycji.

3. Zbuduj formularz reaktywny do aktualizacji nowego rekordu dla obiektu zadania do realizacji `Todo` (pola tytuł - input typu text, czy zakończone zadanie - checkbox, user id - select z wyborem użytkownika). Jeżeli zadanie nie zostało jeszcze zakończone to istnieje możliwość edycji i zapisania zmian, jeżeli zostało zakończone to użytkownik może zmienić wszystkie dane.

4. Wykorzystaj wbudowane walidatory required, maxlength, minlength na polach.

5. Wyświetl błędy walidacji wraz ze szczegółem jaki błąd wystąpił.

6. Zapewnij by formularz nie będzie submitowany w momencie kiedy walidacja nie została spełniona.

7. Napisz serwis (jeżeli go nie ma) oraz żądanie PUT wysyłające zaktualizowane zadanie do realizacji pod adres url endpointu.
`https://jsonplaceholder.typicode.com/todos`
