# Проект по Сегментации Изображений с Проблемами Кожи [RU]
#
## Введение
Этот проект посвящен решению задачи сегментации изображений с проблемами кожи. Для достижения наилучших результатов было проведено множество экспериментов, в том числе использование различных моделей и функций потерь. В данном README представлены краткие описания трех архитектур: SegNet, UNet и UNet2, а также приведены примеры использования и обучения моделей.

## SegNet
### Архитектура
Модель SegNet основана на архитектуре кодировщик-декодировщик с пропускными соединениями. Кодировщик уменьшает размер входного изображения с помощью сверточных и слоев максимального пулинга, в то время как декодировщик увеличивает размер карт признаков для создания маски сегментации. Между сверточными слоями применяются нормализация по батчу и функции активации ReLU.
#
## UNet
### Архитектура
Модель UNet - это популярная архитектура для сегментации изображений, представляющая собой кодировщик-декодировщик с пропусками. Кодировщик уменьшает пространственные размеры через сверточные и слои максимального пулинга, а декодировщик увеличивает карты признаков для создания окончательной маски сегментации. В модели используются нормализация по батчу и функции активации ReLU между сверточными слоями.
# 
## UNet2
### Архитектура
UNet2 представляет собой вариант модели UNet с измененным дизайном кодировщика. В этой архитектуре для уменьшения размеров используются сверточные слои с пропусками. Декодировщик затем выполняет увеличение размеров через транспонированные сверточные слои для создания маски сегментации. Модель также включает в себя нормализацию по батчу и функции активации ReLU.
#
## Вывод
Наилучших результатов мы достигли, использую архитектуру UNet (Unet2).<br>
При этом UNet сумела достичь самой высокой точности при меньшем количестве итераций.
#
#
#
# Skin Issues Image Segmentation Project
## Introduction
This project is dedicated to solving the problem of image segmentation with skin issues. To achieve the best results, numerous experiments were conducted, including the use of various models and loss functions. In this README, brief descriptions of three architectures—SegNet, UNet, and UNet2—are provided, along with examples of using and training the models.

## SegNet
### Architecture
The SegNet model is based on an encoder-decoder architecture with skip connections. The encoder reduces the size of the input image using convolutional and max-pooling layers, while the decoder increases the feature map size to create a segmentation mask. Batch normalization and ReLU activation functions are applied between convolutional layers.

## UNet
### Architecture
The UNet model is a popular architecture for image segmentation, representing an encoder-decoder with skip connections. The encoder reduces spatial dimensions through convolutional and max-pooling layers, while the decoder increases feature maps to create the final segmentation mask. Batch normalization and ReLU activation functions are used between convolutional layers.

## UNet2
### Architecture
UNet2 is a variant of the UNet model with a modified encoder design. In this architecture, skip connections are implemented using convolutional layers. The decoder then performs upsampling through transposed convolutional layers to create the segmentation mask. The model also includes batch normalization and ReLU activation functions.

## Conclusion
The best results were achieved using the UNet (UNet2) architecture.<br>
UNet demonstrated the highest accuracy with fewer iterations.
