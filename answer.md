# Задача 1  
### Последнее значение цикла  
![image](https://user-images.githubusercontent.com/113675674/209465556-18fed7e9-b8ed-4d01-b514-f894bded9904.png)  
Каждое выполнение цикла уменьшает i. Проверка while(i) остановит цикл при i = 0.  

Соответственно, будет такая последовательность шагов цикла («развернём» цикл):  
![image](https://user-images.githubusercontent.com/113675674/209465563-ed8d37fd-4517-49eb-86c6-faeb49f7b81a.png)  


# Задача 2  
Задача демонстрирует, как постфиксные/префиксные варианты могут повлиять на результат, когда используются в сравнениях.  
![image](https://user-images.githubusercontent.com/113675674/209465892-80cd28ea-fc57-4248-bae3-1324fb5e9a8f.png)  
Первое значение: i = 1, так как операция ++i сначала увеличит i, а потом уже произойдёт сравнение и выполнение alert.   
Далее 2, 3, 4… Значения выводятся одно за другим. Для каждого значения сначала происходит увеличение, а потом – сравнение, так как ++ стоит перед переменной.   
При i = 4 произойдёт увеличение i до 5, а потом сравнение while (5 < 5) – это неверно. Поэтому на этом цикл остановится, и значение 5 выведено не будет.  
![image](https://user-images.githubusercontent.com/113675674/209465930-f8f2a032-813c-49ff-b752-1eed849fc510.png)  
Первое значение: i = 1. Остановимся на нём подробнее. Оператор i++ увеличивает i, возвращая старое значение, так что в сравнении i++ < 5 будет участвовать старое i = 0.  
Но последующий вызов alert уже не относится к этому выражению, так что получит новый i = 1.  
Далее 2, 3, 4… Для каждого значения сначала происходит сравнение, а потом – увеличение, и затем срабатывание alert.  
Окончание цикла: при i = 4 произойдёт сравнение while (4 < 5) – верно, после этого сработает i++, увеличив i до 5, так что значение 5 будет выведено. Оно станет последним.  
Значение i = 5 последнее, потому что на следующем шаге while (5 < 5) ложно.  

# Задача 3  
![image](https://user-images.githubusercontent.com/113675674/209474575-12e88a9b-dc9b-4950-9633-af276ec4f200.png)  
Такой результат обусловлен алгоритмом работы for:  
Выполнить единожды присваивание i = 0 перед чем-либо (начало).  
Проверить условие i < 5  
Если true – выполнить тело цикла alert(i), и затем i++  
Увеличение i++ выполняется отдельно от проверки условия (2), значение i при этом не используется, поэтому нет никакой разницы между i++ и ++i.  

# Задача 4  
###  Выведите чётные числа  
Для проверки на чётность мы здесь используем оператор получения остатка от деления %.  
![image](https://user-images.githubusercontent.com/113675674/209534715-93c9b4be-0cea-4566-88a1-a3b357e83f50.png)  


# Задача 5  
![image](https://user-images.githubusercontent.com/113675674/209534923-73c7d363-adf8-4f06-9aa8-3c90b4ddb72c.png)  

# Задача 6  
![image](https://user-images.githubusercontent.com/113675674/210328857-27aed7a1-f37a-40db-974a-2e0b38d11ba4.png)  

# Задача 7 
![image](https://user-images.githubusercontent.com/113675674/210329555-1a9ab8cd-5024-4d89-90f3-aae50f133dd7.png)  

# Задача 8   
![image](https://user-images.githubusercontent.com/113675674/210329704-d20a6ba9-c4de-4100-9378-c8233eb4ac39.png)  

# Задача 9  
![image](https://user-images.githubusercontent.com/113675674/210329821-811cdf1b-e050-4fe0-b2b8-917fe24feef7.png)


# Задача 10  
![image](https://user-images.githubusercontent.com/113675674/231115796-4515b32a-f53c-458e-8833-77a03df26aaa.png)  


# Задача 11  
![image](https://user-images.githubusercontent.com/113675674/231115842-c60f5b8e-81b8-4453-9435-aec0277f08fe.png)  
В этом решении мы сначала используем функцию parseInt  (можно воспользоваться унарным плюсом) для преобразования введенной пользователем строки в целое число и сохраняем его в переменной number. Затем мы используем цикл for для перебора чисел от 1 до number. На каждой итерации цикла мы выводим в консоль значение текущей переменной цикла, увеличенной на 10.  


# Задача 12  
![image](https://user-images.githubusercontent.com/113675674/231115949-83924b96-144e-47fe-9c84-95d662908175.png)  


# Задача 13   
![image](https://user-images.githubusercontent.com/113675674/231115991-1081d730-157a-4cd8-9be0-34f32a2cb3f4.png)  
В этом решении мы сначала используем функцию parseInt (можно воспользоваться унарным плюсом) для преобразования введенных пользователем строк в целые числа и сохраняем их в переменных start и end. Затем мы инициализируем переменную sum со значением 0, которая будет использоваться для хранения суммы всех нечетных чисел в диапазоне, и используем цикл for для перебора всех чисел в диапазоне от start до end. Внутри цикла мы проверяем, является ли текущее число нечетным с помощью оператора % и, если да, добавляем его к переменной sum. В конце мы выводим в консоль сообщение с результатом.   
