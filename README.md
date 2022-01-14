# IVision2

Структура проекта:
```python
IVision2:
    experiments:
        ClassificationBaseline_ivision_train.ipynb
        ClassificationBaseline_ivision_inference.ipynb
    models:
        ViT_B_32_epoch_2.pth(так как на гит не лезет, доступно по сслыке https://getfile.dokpub.com/yandex/get/https://disk.yandex.ru/d/CHnmggS2yBp02Q)
    ...
```

Решение необходимо запускать с видеокартой.

Все решения проверены на Google Colab.

Блокнот ClassificationBaseline_ivision_inference.ipynb отвечат за предсказания,
Блокнот ClassificationBaseline_ivision_train.ipynb отвечает за тренировку модели.

Для предсказания аварии на видео необходимо создать тестовый файл.

Для создания тестового файла, следуйте следующей структуре:
```python
структура файла test.zip:
    test:
        1.mp4
        2.mp4
        ...
```
Далее необходимо загрузить тестовый файл на гугл диск. 
После загрузки и запуска блокнота для предсказаний, замените ссылку gdown
первой ячейки "Загрузка данных" на свою.

Например, после открытия доступа к файлу вы получили слудющую ссылку.\
https://drive.google.com/file/d/1QrhoG_HEcl9B-BHGFjLEFKOpkdgMKKZy/view?usp=sharing \
Должно получится:\
https://drive.google.com/uc?id=1QrhoG_HEcl9B-BHGFjLEFKOpkdgMKKZy

После выполнения блокнота инференса, выводяться данные о загруженных видео.

False обозначает, что ДТП небыло, True - было.

Дополнительные файлы, а такжее копии из этого репозитория + модель [здесь](https://drive.google.com/drive/folders/11NHKVIPrEKfK7Ao8mlnJMLnnJQtmTwNu?usp=sharing).
