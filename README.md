# Katzen- und Hunde-Klassifizierungsmodell - Custom CNN

Dieses Jupyter Notebook enthält den Code für ein Machine Learning-Modell, das darauf trainiert ist, zwischen Bildern von Hunden und Katzen zu unterscheiden. Es verwendet Convolutional Neural Networks (CNNs), um die Bilder zu verarbeiten und die Klassifizierung durchzuführen. Dieses Modell wurde mit TensorFlow und Keras implementiert.

## Voraussetzungen

Um dieses Notebook auszuführen, stellen Sie sicher, dass Sie folgende Bibliotheken installiert haben:
- NumPy
- OpenCV
- Matplotlib
- Seaborn
- TensorFlow
- Keras

Diese Bibliotheken können über pip installiert werden, indem Sie den folgenden Befehl in Ihrem Terminal ausführen:

pip install numpy opencv-python matplotlib seaborn tensorflow keras

## Modellarchitektur

Das Modell besteht aus mehreren Schichten, einschließlich Convolutional Layers, MaxPooling Layers, Dropout Layers und Dense Layers. Die Architektur ist wie folgt aufgebaut:
1. Conv2D-Schichten für die Feature-Extraktion aus den Bildern.
2. MaxPooling-Schichten zur Reduzierung der Dimensionalität.
3. Dropout-Schichten zur Vermeidung von Overfitting.
4. Dense Layers zur Klassifizierung.

## Training des Modells

Das Modell wird mit Bildern von Hunden und Katzen trainiert. Das Training umfasst auch Data Augmentation, um die Vielfalt des Trainingsdatensatzes zu erhöhen und das Modell robuster zu machen.

## Callbacks

Zwei wichtige Callbacks werden verwendet:
1. `EarlyStopping`: Stoppt das Training frühzeitig, wenn sich die Genauigkeit auf den Validierungsdaten nicht verbessert.
2. `ReduceLROnPlateau`: Reduziert die Lernrate, wenn sich die Genauigkeit auf den Validierungsdaten nicht verbessert, um feinere Anpassungen zu ermöglichen.

## Ausführung

Um das Modell zu trainieren und zu evaluieren, führen Sie einfach alle Zellen des Notebooks der Reihe nach aus.

## Ergebnisse

Die Ausgabe des Notebooks umfasst die Genauigkeit und den Verlust des Modells während des Trainings und der Validierung.
9 zufällig ausgewählte Bilder werden von dem Model klassifiziert.
