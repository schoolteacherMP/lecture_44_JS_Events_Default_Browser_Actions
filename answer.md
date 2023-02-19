## Задача 1.   
### Почему не работает return false?  
Когда браузер считывает атрибут on*, например onclick, он создаёт функцию-обработчик с содержимым этого атрибута в качестве тела функции.  

Функция для onclick="handler()" будет:  
![image](https://user-images.githubusercontent.com/113675674/219848145-7f096380-6296-4ecb-a18d-7b420bb623c5.png)  

Сейчас нам видно, что возвращаемое значение handler() не используется и не влияет на результат.  

Исправить очень просто:  
![image](https://user-images.githubusercontent.com/113675674/219848157-dce68e12-dba8-4e08-9090-5bd917ea8630.png)  

Также мы можем использовать event.preventDefault(), например:  
![image](https://user-images.githubusercontent.com/113675674/219848171-a907fd06-bbc1-4152-8eb0-3a38cb2f69f2.png)  



## Задача 2.   
### Галерея изображений  
Примеры вариантов решения:  
![image](https://user-images.githubusercontent.com/113675674/219934182-443fdd81-6992-4a47-803e-4b6e8ac4ddbd.png)  

![image](https://user-images.githubusercontent.com/113675674/219934197-1d16d935-2b35-4acf-83fd-63a6e3bea9d2.png)

