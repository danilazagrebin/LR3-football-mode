# LR3-football-mode
·	Создайте новый пустой 3D проект на Unity.

·	Скачайте папку с ML агентом по [ссылке](https://disk.yandex.ru/d/mIw-B-VaHllwdg)

·	В созданный проект добавьте ML Agent, выбрав Window - Package Manager - Add Package from disk. Последовательно добавьте .json – файлы:

o	ml-agents-release_19 / com,unity.ml-agents / package.json

o	ml-agents-release_19 / com,unity.ml-agents.extensions / package.json

·	Если все сделано правильно, то во вкладке с компонентами (Components) внутри Unity вы увидите строку ML Agent.

·	Далее запускаем Anaconda Prompt от имени администратора для возможности запуска команд через консоль.

·	Далее пишем серию команд для создания и активации нового ML-агента, а также для скачивания необходимых библиотек:

o	mlagents 0.28.0;

o	torch 1.7.1;

![image](https://user-images.githubusercontent.com/114522298/207288815-7502d2ba-2283-4ebf-a88f-cde84cdf5fe0.png)
![image](https://user-images.githubusercontent.com/114522298/207288844-925ce2e8-3a3f-4e0c-8ae7-5aba5bb980a7.png)
![image](https://user-images.githubusercontent.com/114522298/207288874-7e424ae1-569d-4267-a531-0604da4d8ea8.png)
![image](https://user-images.githubusercontent.com/114522298/207288900-e9ceaec6-cc18-49ed-bf1a-89a4bbb8a92d.png)



·	Создайте на сцене плоскость, ворота и сферу так, как показано на рисунке ниже. Модель ворот можно взять в файлах репозитория. 

· Создайте новый материал для поля, задайте зелёный цвет в свойствах материала и перетащите материал на плоскость (right click->Create->New material)

· Создайте новый материал для мяча, скачайте текстуру из файлов репозитория, перетащите текстуру на параметр материала albedo 


![image](https://user-images.githubusercontent.com/114522298/207294963-67373f99-e1f0-4732-9b67-25fc61aea3ef.png)

· Для модели ворот добавьте компонент Box colider. Настройте его, как показано ниже

![image](https://user-images.githubusercontent.com/114522298/207304844-b13e1dbb-5b1a-408f-b635-575d58c47023.png)


·	Создайте простой C# скрипт-файл и подключите его к сфере:

·	В скрипт-файл RollerAgent.cs добавьте код, опубликованный в файлах репозитория. В данном файле описан поворот ворот в сторону мяча, а так же движение мяча к воротам.

·	Объекту «сфера» добавьте компоненты Rigidbody, Decision Requester, Behavior Parameters и настройте их так, как показано на рисунке ниже:

 ![image](https://user-images.githubusercontent.com/114522298/207300335-eed85997-9872-4c03-af05-9ff08db0de15.png)
 
·	В корень проекта добавьте файл конфигурации нейронной сети, доступный в папке с файлами проекта по [ссылке](https://disk.yandex.ru/d/n-vSx2vhvvrA6A), также его можно скачать из файлов репозитория
  
·	Запустите работу ml-агента
![image](https://user-images.githubusercontent.com/114522298/207301809-f3b339cc-681a-481a-ac25-b9d5bb72d3a0.png)

·	Запустите сцену и обучение в консоли Anaconda. Для достижения большей эффективности необходимо маштабировать количество платформ.
  - После достижения удовлетворительного результата можно остановить симуляцию в Unity и Anaconda. После остановки убираем лишние платформы и запускаем игру.
  - В результате должно получиться резултат схожий с этим:
![2022-12-11 14-29-33](https://user-images.githubusercontent.com/114522298/207304062-1c471311-ea78-4ce6-9780-ec337e400acd.gif)

Ссылка на архив с проектом - [проект](https://disk.yandex.ru/d/MfghtR0mQBDS8w)

Работу выполнили:
  - Загребин Данила Павлович, студент РИ-212702
  - Шлыков Олег Петрович, студент РИ-212702
