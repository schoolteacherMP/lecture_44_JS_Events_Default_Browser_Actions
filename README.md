# lecture_44_JS_Events_Default_Browser_Actions  
#  [Задачи ](https://github.com/schoolteacherMP/lecture_44_JS_Events_Default_Browser_Actions/blob/main/tasks.md)  

Действий браузера по умолчанию достаточно много:  

-  **mousedown** – начинает выделять текст (если двигать мышкой).  
-  **click** на `<input type="checkbox">` – ставит или убирает галочку в input.  
-  **submit** – при нажатии на `<input type="submit">` или при нажатии клавиши Enter в форме данные отправляются на сервер.  
-  **keydown** – при нажатии клавиши в поле ввода появляется символ.  
-  **contextmenu** – при правом клике показывается контекстное меню браузера.  
-  …и многие другие…  

Все эти действия можно отменить, если мы хотим обработать событие исключительно при помощи JavaScript.  

Чтобы отменить действие браузера по умолчанию, используйте **event.preventDefault()** или return false. Второй метод работает, только если обработчик назначен через `on<событие>`.  

Опция **passive**: true для addEventListener сообщает браузеру, что действие по умолчанию не будет отменено. Это очень полезно для некоторых событий на мобильных устройствах, таких как touchstart и touchmove, чтобы сообщить браузеру, что он не должен ожидать выполнения всех обработчиков, а ему следует сразу приступать к выполнению действия по умолчанию, например, к прокрутке.  

Если событие по умолчанию отменено, то значение **event.defaultPrevented** становится true, иначе false.  

