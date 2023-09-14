### Задание: 
#### Необходимо продемонстрировать изоляцию одного и того же приложения (как решено на семинаре - командного интерпретатора) в различных пространствах имен.

Создаем каталог "testfolder" в домашнем каталоге
![picrure1](https://github.com/MarkovaOlga/Containerization_Hometask1/blob/main/pictures/sc1.jpg)

Скопируем необходимые файлы в новую папку
![picture2](https://github.com/MarkovaOlga/Containerization_Hometask1/blob/main/pictures/sc02.jpg)

Смотрим, какие библиотеки необходимо добавить, создаем для них папки и копируем их в новые папки
![picture3](https://github.com/MarkovaOlga/Containerization_Hometask1/blob/main/pictures/sc03.jpg)

Вводим команду chroot.
Теперь мы находимся в изолированной среде
![picture4](https://github.com/MarkovaOlga/Containerization_Hometask1/blob/main/pictures/sc04.jpg)

Чтобы в этой среде работали другие команды, нам также надо скопировать соответствующие файлы и библиотеки
![picture5](https://github.com/MarkovaOlga/Containerization_Hometask1/blob/main/pictures/sc5.jpg)

Теперь создадим пространство имен для сети.
Для этого воспользуемся командой ip. Создадим пространство имен с именем "testns"
![picture6](https://github.com/MarkovaOlga/Containerization_Hometask1/blob/main/pictures/sc06.jpg)

Таким образом мы создали изолированное сетевое окружение.
Использую команду ip, мы можем выполнить процесс в созданном пространстве имен и проверить, как теперь работают команды
![picture7](https://github.com/MarkovaOlga/Containerization_Hometask1/blob/main/pictures/sc07.jpg)

Используя утилиту unshare, мы можем что-то разграничивать и создавать пространство имен по этим ограничениям
![picture8](https://github.com/MarkovaOlga/Containerization_Hometask1/blob/main/pictures/sc08.jpg)
![picture9](https://github.com/MarkovaOlga/Containerization_Hometask1/blob/main/pictures/sc09.jpg)
