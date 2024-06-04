Дипломная работа на тему: «Детекция эмоций человека»

Исходной задачей работы является реализация искусственной нейронной сети с использованием компьютерного зрения для классификации и детекции объектов. Вторая часть — это определение на видео в режиме реального времени эмоции субъектов. Объекты детекции лица людей, классификация — определение 7 эмоций. Архитектура модели – CNN.

Датасет: «FER2013» https://www.kaggle.com/datasets/ashishpatel26/facial-expression-recognitionferchallenge/data Количество изображений: 35887 шт. Количество классов: 7 Классы: anger, disgust, fear, happiness, sadness, surprise, neutral Описание: Данные состоят из изображений лиц размером 48x48 пикселей в оттенках серого. Столбец «emotion» содержит числовой код от 0 до 6 включительно для эмоции, присутствующей на изображении. Столбец «pixels» содержит строку, заключенную в кавычки для каждого изображения. Содержимое этой строки представляет собой значения пикселей, разделенные пробелами, в порядке возрастания строк.

Варианты исследований модели CNN, применяемых в работе: Модель CNN, активация ReLu, активация ELU

As is (как есть). Т.е. модель обучалась на данных без весов класса (class_weight) CNN_1_asis.ipynb • https://github.com/dubovik-alexander/Netology-DS/blob/main/Diploma/final/py_files/CNN_1_asis.ipynb - активация «ReLU» • https://github.com/dubovik-alexander/Netology-DS/blob/main/Diploma/final/py_files/CNN_1_asis_elu_.ipynb - активация «ELU»

Обучение модели с учетом весов класса. • https://github.com/dubovik-alexander/Netology-DS/blob/main/Diploma/final/py_files/CNN_2_weight_colab.ipynb - активация «ReLU» • https://github.com/dubovik-alexander/Netology-DS/blob/main/Diploma/final/py_files/CNN_2_weight_elu_colab.ipynb - активация «ELU»

Обучение модели с процессом переобучения данных с использованием метода Synthetic Minority Over-sampling Technique (SMOTE) для решения проблемы дисбаланса классов в наборе данных. • https://github.com/dubovik-alexander/Netology-DS/blob/main/Diploma/final/py_files/CNN_4_weight_oversampling_relu_colab.ipynb - активация «ReLU» • https://github.com/dubovik-alexander/Netology-DS/blob/main/Diploma/final/py_files/CNN_4_weight_oversampling_elu_colab.ipynb - активация «ELU»

Проводились исследования влияние функции активации ReLu и ELU на точность обучения модели. 
