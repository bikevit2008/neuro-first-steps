# neuro-first-steps

KNN(по соседям):
1. 96.88% дефолт
2. 96.65% knn_classifier = KNeighborsClassifier(n_jobs=-1, n_neighbors=10)
3. 97.05%  knn_classifier = KNeighborsClassifier(n_jobs=-1, n_neighbors=3)


SGD:
1. 87.94% sgd_classifier = SGDClassifier(n_jobs=-1, tol=0.0001)
2. 85.94000000000001% sgd_classifier = SGDClassifier(n_jobs=-1, tol=0.0001, penalty="elasticnet")
3. 88.34% sgd_classifier = SGDClassifier(n_jobs=-1, tol=0.0001, penalty="elasticnet", l1_ratio=0.10)
4. 86.48% sgd_classifier = SGDClassifier(n_jobs=-1, tol=0.0001, penalty="elasticnet", l1_ratio=0.05)


Нейросети:
1. 96.17999999999999% Дефолт
2. 11.35% MLPClassifier(hidden_layer_sizes=(784, 800, 10), verbose=True)
3. 96.94% nn_classifier = MLPClassifier(hidden_layer_sizes=(784, 800), verbose=True)
4. 97.75% nn_classifier = MLPClassifier(hidden_layer_sizes=(784, 800), verbose=True)


Узнал, что на одной и той же выборке данных, на одних и тех же аргументах нейросеть учится по-разному
SGD гораздо быстрее делает prediction для всех образцов, чем KNN

Пробил предел точности метода k ближайщих соседей

Мои выводы чисто практические могут на других выборках данных и при других условиях быть неверными или отличающимися. Мне недостаточно опыта, чтобы предусмотреть сценарии более широко.

Примечание: я дублировал один и тот же файл со второго дня для записи разных данных, можно было сделать все в одном, возможно написать функцию, но мне было лень, запуск проще нажать. Я думаю, что вам будут нужны конкретные результаты (пруфы) - они есть.
