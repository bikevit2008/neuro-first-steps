# neuro-first-steps

KNN(по соседям):
1. 96.88% дефолт
2. 96.65% knn_classifier = KNeighborsClassifier(n_jobs=-1, n_neighbors=10)
3. 97.05%  knn_classifier = KNeighborsClassifier(n_jobs=-1, n_neighbors=3)


Нейросети:
1. 96.17999999999999% Дефолт
2. 11.35% MLPClassifier(hidden_layer_sizes=(784, 800, 10), verbose=True)
3. 96.94% nn_classifier = MLPClassifier(hidden_layer_sizes=(784, 800), verbose=True)
4. 97.75% nn_classifier = MLPClassifier(hidden_layer_sizes=(784, 800), verbose=True)

Узнал, что на одной и той же выборке данных, на одних и тех же аргументах нейросеть учится по-разному

Пробил предел точности метода k ближайщих соседей

Примечание: я дублировал один и тот же файл со второго дня для записи разных данных, можно было сделать все в одном, возможно написать функцию, но мне было лень, запуск проще нажать. Я думаю, что вам будут нужны конкретные результаты (пруфы) - они есть.
