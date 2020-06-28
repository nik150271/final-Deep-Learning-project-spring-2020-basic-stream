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
