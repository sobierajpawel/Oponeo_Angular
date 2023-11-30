---------------------------------------------------------------------------------------------------------------------------------------------------
pl

# Utworzenie generycznego komponentu do potwierdzania usuwania.

1. Zbuduj komponent odpowiedzialny za ukazywanie okna dialogowego.

```html
<div *ngIf="message && message.message != ''" class="modal" tabindex="-1" role="dialog" style="display:block!important">    
    <div class="modal-dialog modal-dialog-centered" role="document">    
        <div class="modal-content">    
            <div class="modal-header">
                <h5 class="modal-title" id="exampleModalLongTitle">Potwierdzenie operacji</h5>
              </div>
            <div class="modal-body">    
                <div class="row">    
                    <div class="col-md-12">    
                        <p class="text-center">{{message.message}}</p>    
                    </div>    
                </div>    
                <div class="row">    
                    <div class="col-md-12">    
                        <p class="confirm-button">    
                            <a class="mr-2" (click)="onAccept()">    
                                <button class="btn btn-success">Tak</button>    
                            </a>    
                            <a (click)="onCancel()">    
                                <button style="margin-left:10px" class="btn btn-danger">Nie</button>    
                            </a>    
                        </p>    
                    </div>    
                </div>    
            </div>    
        </div>    
    </div>    
</div>    
```

2. Wykorzystaj obiekt, który będzie wykorzystywany do przesyłania komunikatu, funkcji do pozytywnej i negatywnej odpowiedzi użytkownika w oknie.

```ts
export class ConfirmMessage {
    message: string = "";
    yesFn!: () => void;
    noFn: () => void = () => {};
}
```

3. Zbuduj serwis do przesyłania komunikatów z wykorzystaniem RxJS oraz obiektu `Subject`.

4.  Nie zapomnij użyć komponentu okna dialogowego w głównym komponencie aplikacji.

---------------------------------------------------------------------------------------------------------------------------------------------------
en

# Creating a Generic Component for Delete Confirmation

1. Build a component responsible for displaying the dialog window.

```html
<div *ngIf="message && message.message != ''" class="modal" tabindex="-1" role="dialog" style="display:block!important">    
    <div class="modal-dialog modal-dialog-centered" role="document">    
        <div class="modal-content">    
            <div class="modal-header">
                <h5 class="modal-title" id="exampleModalLongTitle">Potwierdzenie operacji</h5>
              </div>
            <div class="modal-body">    
                <div class="row">    
                    <div class="col-md-12">    
                        <p class="text-center">{{message.message}}</p>    
                    </div>    
                </div>    
                <div class="row">    
                    <div class="col-md-12">    
                        <p class="confirm-button">    
                            <a class="mr-2" (click)="onAccept()">    
                                <button class="btn btn-success">Tak</button>    
                            </a>    
                            <a (click)="onCancel()">    
                                <button style="margin-left:10px" class="btn btn-danger">Nie</button>    
                            </a>    
                        </p>    
                    </div>    
                </div>    
            </div>    
        </div>    
    </div>    
</div>    
```
2. Utilize an object that will be used to transmit the message, functions for positive and negative user responses in the window.

```ts
export class ConfirmMessage {
    message: string = "";
    yesFn!: () => void;
    noFn: () => void = () => {};
}
```

3. Build a service for transmitting messages using RxJS and the Subject object.

4. Don't forget to use the dialog window component in the main component of the application.
