# final-Deep-Learning-project-spring-2020-basic-stream
Submission of the final Stepik project. Task of segmentation of a custom dataset (a stack of boards) using Detectron2.

## Для задачи сегментации был выбран второй сценарий (работа с собственным Датасетом)
По этапам работы
1. Выбрал фреймворк Detectron2
2. Проверил его работу на Воздушных шарах
3. Для проекта решил создать свой датасет - штабеля досок
4. Выбрал для train - 83 изображения, для val - 22 изображения. При помощи CVAT сделал сегментацию.
![alt text](https://github.com/nik150271/final-Deep-Learning-project-spring-2020-basic-stream/blob/master/Img/stack-segmentation.jpg)
Для 83 изображений получилось 199 масок.
Написал get_stack_dicts - создание словаря для Dataloader Detectron2
К сожалению не успел разобраться с Аугментацией для Detectron2, поэтому обучение было на 83 изображениях.
5. Произвел обучение модели (model_zoo), поэксперементировал с параметрами.
6. Качество работы модели можно посмотреть с помощью inference_on_dataset.

Все вышеописанное есть в Ноутбуке в папке Notebook.
Данные val и train залиты на мой гугл диск. При работе я его монтирую и получаю туда доступ.
Для проверки работы я расшарил директорию, где находятся две папки val и train ( https://drive.google.com/drive/folders/1_bMIIiEXQ74UH3tUgGsMGAqKXuz2RhC2?usp=sharing )

7. Пути применения в бизнесе: добавив сегментацию досок в штабеле (не успел к сожалению), можно создать приложение, которое по фотографии считает количство штабелей и количество досок в каждом штабеле.
