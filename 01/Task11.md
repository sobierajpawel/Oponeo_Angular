# Input/Output komunikacja rodzic <-> dziecko

1. Zbuduj strukturę komponentów, która pozwoli na wyświetlenie szczegółów użytkownika. Utwórz komponenty:
- komponent rodzica, w którym będą realizowane operacje pobierania danych 
- komponent dziecka, który będzie odpowiedzialny za wyświetlenie szczegółów użytkownika - jego imienia i nazwiska, adres mailowego,
strony internetowej, informacji czy jest aktywny czy też nie,
- komponent dziecka, w którym znajdą się wszystkie zadania do realizacji wyświetlone w formie listy/tabeli
- komponentu dziecka, w którym będą znajdowały się przyciski - przekierowania do edycji użytkownika (przycisk edytuj), powrotu do poprzedniego
widoku (przycisk powrót).

2. Komponent rodzica ma obsługiwać pobieranie danych i przesyłania ich do komponentów dzieci. Dodatkowo logika obsługi 
metod powrotu oraz edycji musi znajdować się w komponencie rodzica.

3. Do pobrania listy zadań wykorzystaj endpoint.

```https://jsonplaceholder.typicode.com/users/5/todos```

4. Do komunikacji wykorzystaj dekoratory `Input()` `Output()`.
