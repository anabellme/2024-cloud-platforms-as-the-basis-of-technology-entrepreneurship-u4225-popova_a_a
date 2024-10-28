**University**: [ITMO University](https://itmo.ru/ru/)

**Faculty**: [FTMI](https://ftmi.itmo.ru/)

**Course**: [Cloud platforms as the basis of technology entrepreneurship](https://itmo-ict-faculty.github.io/cloud-platforms-as-the-basis-of-technology-entrepreneurship/) 

**Year**: 2024

**Group**: U4225

**Author**: Popova Anna Andreevna

**Lab**: Lab3

**Date of create**: 28.10.2024

**Date of finished**: 28.10.2024

# Лабораторная работа №3: "Исследование Cloud Run"

## Цель работы:

Познакомиться с функционалом **Google Cloud Storage**, создать и настроить хранилище для объектов, научиться загружать, перемещать и управлять доступом к файлам в облачном хранилище.

## Ход работы:

### 1. Выбор проекта

Выбрала существующий проект с необходимыми разрешениями **`cloud-platforms-as-the-basis`**.

<img width="1116" alt="image" src="https://github.com/user-attachments/assets/6e13766f-a8fc-4a9e-b0ec-946041b4f3b5">

### 2. Создание Cloud Storage bucket

- Перешла в Google Cloud Console и выбрала раздел **Сloud Storage**;
- Нажала **Create Bucket** и указала название для нового бакета;
- Выбрала расположение бакета (**ue**) и класс хранения данных (**Standard**).

<img width="1710" alt="image" src="https://github.com/user-attachments/assets/36650707-ade6-46cc-b1e7-0dcc559ebd8f">

Был создан пустой Cloud Storage bucket, готовый для загрузки и хранения файлов.

### 3. Загрузка изображений в Cloud Storage bucket

В созданном бакете выбрала **Upload Files** и загрузила 3 изображения со своего компьютера. 

<img width="1480" alt="image" src="https://github.com/user-attachments/assets/5905c6d0-0556-434b-bc43-a849c5670a8b">

Файлы успешно загрузились и отобразились в интерфейсе бакета.

### 4. Создание папки и перемещение файлов

- В интерфейсе бакета нажала **Create Folder** и создала папку **cats**
- После создания папки выделила загруженные файлы и переместила их в созданную папку с помощью опции **Move** в контекстном меню.

<img width="1478" alt="image" src="https://github.com/user-attachments/assets/a7297d8a-4f3f-4231-98f6-08ce17a36e13">

Все изображения перемещены в папку **`images-folder`** внутри бакета, что помогает структурировать файлы.

### 5. Настройка публичного доступа к файлам

- Для каждого загруженного файла открыла настройки доступа;
- В разделе **Permissions** добавила новую роль для объекта — указала **allUsers** в качестве пользователя и предоставила ему **Viewer** доступ;
- Подтвердила изменения, чтобы файлы стали публично доступными.

<img width="472" alt="image" src="https://github.com/user-attachments/assets/5619ff64-ad74-4d54-9075-13e85dacd063">

Файлы в бакете теперь имеют публичный доступ, что позволяет просматривать их без авторизации.

<img width="1479" alt="image" src="https://github.com/user-attachments/assets/8ce61c6c-9d43-42ad-868b-36d7fa08fe19">

### 6. Создание ссылок на файлы

- Для каждого файла открыла контекстное меню и выбрала **Copy URL**. Это создало **публичные ссылки** для всех загруженных файлов.
- Переход по этим ссылкам из любого браузера подтверждает доступ к изображениям.

https://storage.googleapis.com/apopovalab3/cats/beautiful-kitten-with-colorful-clouds_23-2150752964.jpg.avif
https://storage.googleapis.com/apopovalab3/cats/cute-kitten-clouds_23-2150752838.jpg.avif
https://storage.googleapis.com/apopovalab3/cats/view-3d-adorable-cat-with-fluffy-clouds_23-2151113419.jpg.avif

Были созданы прямые ссылки на изображения, которые можно использовать для просмотра файлов.

## Выводы

В процессе работы с Google Cloud Storage были достигнуты следующие результаты:

- Создан бакет для хранения файлов с возможностью задания уровня доступа;
- Загружены и структурированы файлы внутри бакета;
- Настроен публичный доступ к файлам, что позволяет легко делиться ссылками;
- Изучены ключевые операции **Cloud Storage**, такие как создание бакета, загрузка файлов, настройка прав доступа и удаление.

Cloud Storage позволяет гибко управлять файлами в облаке, поддерживая как приватные, так и публичные уровни доступа. Благодаря этим возможностям данный сервис отлично подходит для хранения данных любого типа — от часто запрашиваемых до архивных данных, предлагая широкий выбор классов хранения и удобный интерфейс для управления доступом.





