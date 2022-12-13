# LR3-football-mode
·	Создайте новый пустой 3D проект на Unity.

·	Скачайте папку с ML агентом. Вы найдете ее в облаке с исходными файлами к лабораторной работе – ml-agents-release_19.

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



 ![image](https://user-images.githubusercontent.com/114522298/207288694-d128a3f7-3c2b-4b35-add7-aaf8fda4e49c.png)



·	Создайте на сцене плоскость, куб и сферу так, как показано на рисунке ниже. Создайте простой C# скрипт-файл и подключите его к сфере:

