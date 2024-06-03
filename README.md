# Лабораторная работа №2. Вариант 12
### Описание программы
---
Программа предназначена для управления данными о преподавателях университета с помощью графического интерфейса и XML файлов. Реализован функционал поиска и удаления по по фамилии преподавателя(может быть заполнен только один элемент ФИО, например имя);, по наименованию кафедры; 
по ученому званию и факультету;
по стажу работы (задается верхний и нижний предел);


### Демонстрация работы программы
`Главное окно` программы представлено в виде таблицы со столбиками Id, Факультет, Наименование кафедры, ФИО преподавателя, Ученое звание, Ученая степень, Стаж работы. Также на главном окне присутствуют различные кнопки управления (переключение самих страниц) и инструменты для работы с базой (загрузка из файла, сохранение в файл, добавление записи, поиск по фильтру и удаление по фильтру).

![главное окно](https://github.com/KaterinaNemkova/PPOIS2Laba4SEM/blob/main/photo/%D0%B3%D0%BB%D0%B0%D0%B2%D0%BD%D0%BE%D0%B5%20%D0%BE%D0%BA%D0%BD%D0%BE.png)

 ### Работа с данными
 Программа поддерживает работу с видом файла - `.xml`. При загрузке файла программа предлагает, что делать с записями из файла: дообавить их в таблицу или заменить новыми записями старые.
 
 ![загрузка записей](https://github.com/KaterinaNemkova/PPOIS2Laba4SEM/blob/main/photo/%D0%B7%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B0%20%D0%B7%D0%B0%D0%BF%D0%B8%D1%81%D0%B5%D0%B9.png)

 После загрузки программа выводит сообщение об успешной или не успешной загрузке файла.

 ![успешная загрузка](https://github.com/KaterinaNemkova/PPOIS2Laba4SEM/blob/main/photo/%D1%83%D1%81%D0%BF%D0%B5%D1%88%D0%BD%D0%B0%D1%8F%20%D0%B7%D0%B0%D0%B3%D1%80%D1%83%D0%B7%D0%BA%D0%B0.png)

 Также можно загрузить записи в файл `.xml`. После сохранения программа оповестит об успешном/не успешном сохранении. 
 
 ![сохранение](https://github.com/KaterinaNemkova/PPOIS2Laba4SEM/blob/main/photo/%D1%81%D0%BE%D1%85%D1%80%D0%B0%D0%BD%D0%B5%D0%BD%D0%B8%D0%B5.png)
 

### Добавление информации о преподавателе
Для добавления преподавателя необходимо нажать `Добавить запись`. Открывается окно, в котором пользователь может ввести данные о преподавателе.

![add_pet](https://github.com/Mariannnnaaaaa/ppois-2-2024/assets/115795639/78539050-1d41-42a3-ab3d-f33e859ebed9)

Поля Факультет, Наименование кафедры, Ученое звание, Ученая степень можно выбрать из выдвигающегося списка. Также предусмотрен функционал, который после выбора факультета предлагать кафедры 
только для выбранного факультета.

![add_pet](https://github.com/Mariannnnaaaaa/ppois-2-2024/assets/115795639/78539050-1d41-42a3-ab3d-f33e859ebed9)

В данной процедуре добавления обработаны такие ошибки, как:
```
- стаж работы может содержать только цифры
- поля Факультет, Наименование кафедры, ФИО преподавателя, Ученое звание, Ученая степень должны содержать только буквы русского алфавита
- нельзя оставлять пустые поля
```
Пример некорректного ввода:

![add_pet](https://github.com/Mariannnnaaaaa/ppois-2-2024/assets/115795639/78539050-1d41-42a3-ab3d-f33e859ebed9)

![add_pet](https://github.com/Mariannnnaaaaa/ppois-2-2024/assets/115795639/78539050-1d41-42a3-ab3d-f33e859ebed9)

![add_pet](https://github.com/Mariannnnaaaaa/ppois-2-2024/assets/115795639/78539050-1d41-42a3-ab3d-f33e859ebed9)

## Поиск преподавателя
В данной программе реализована логика поиска преподавателя. Результаты поиска преподавателй отображаются в новой таблице, где указывается, сколько преподавателей было найдено или не найдено ни одного. 

![search_by_filter](https://github.com/Mariannnnaaaaa/ppois-2-2024/assets/115795639/41783cfa-3af3-48ca-a508-ae59c4d63a60)


![search_by_filter](https://github.com/Mariannnnaaaaa/ppois-2-2024/assets/115795639/41783cfa-3af3-48ca-a508-ae59c4d63a60)


### Удаление питомца
В данной программе реализована логика удаления преподавателя. Удалять мы можем по заявленным критериям. Критерии могут быть выбраны поодиночке - пользователь сам выбирает необходимый критерий удаления преподавателя. При успешном удалении выводится окно успеха с количеством удаленных записей. При неуспешном сообщается о несуществовании такой записи в таблице. Пустые поля оставлять нельзя. После успешного либо неуспешного удаления поля ввода критерия обнуляются.

![delete](https://github.com/Mariannnnaaaaa/ppois-2-2024/assets/115795639/aa1fc267-fd4b-4c32-ba51-594e06855122)


![delete matches](https://github.com/Mariannnnaaaaa/ppois-2-2024/assets/115795639/8e8bee1c-6572-4562-839f-24b090e12b93)

