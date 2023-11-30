----------------------------------------------------------------------------------------------------------------------------------
pl
# Wykorzystanie dynamicznie tworzonych kontrolek w formularzu reaktywnym

1. Zbuduj komponent, który będzie umożliwiał wybranie jednego użytkownika i dodaniu wielu zadań w ramach jednego formularza oraz ich usuwania.
Przykładowy design zaprezentowano poniżej.

<img width="514" alt="image" src="https://github.com/sobierajpawel/Oponeo_Angular/assets/18425360/0b8dd5f8-6131-47b1-88ac-63bb4707b420">

<img width="508" alt="image" src="https://github.com/sobierajpawel/Oponeo_Angular/assets/18425360/92aa50b4-7181-4e39-9d45-d348e343c688">

2. Dodaj walidację tak by użytkownik musiał podać przynajmniej jedno zadanie oraz aby każde zadanie miało tytuł. Postaraj się użyć
wbudowanych walidatorów `Validators.required`. Opcjonalnie skorzystaj z własnego kodu do takiej walidacji.  

3. Ponieważ API nie obsługuje kolekcji wysyłki kolekcji - wyślij zadania w formie pętli, ale postaraj się wykorzystaj komponent toastów do wyświelenia
potwierdzenia oraz `forkJoin` z biblioteki rxJS to wysłania tylko jednego toasta nawet jeżeli użytkownik wysłał wiele zadań. 

----------------------------------------------------------------------------------------------------------------------------------
en

# Using Dynamically Created Controls in a Reactive Form
1. Build a component that will allow the selection of a single user and the addition of multiple tasks within a single form, as well as their removal. An example design is presented below.

 <img width="514" alt="image" src="https://github.com/sobierajpawel/Oponeo_Angular/assets/18425360/0b8dd5f8-6131-47b1-88ac-63bb4707b420">

<img width="508" alt="image" src="https://github.com/sobierajpawel/Oponeo_Angular/assets/18425360/92aa50b4-7181-4e39-9d45-d348e343c688">

2. Add validation so that the user must provide at least one task and each task must have a title. Try to use the built-in Validators.required validators. Optionally, use your own code for such validation.

3. Since the API does not support sending collections - send the tasks in the form of a loop, but try to use the toast component to display confirmation and forkJoin from the rxJS library to send only one toast even if the user has sent many tasks.
