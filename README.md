# Claws-and-Paws-Sound-Based-Pet-Identification

## Overview

In this project, we focus on classifying environmental sounds as either cat or dog vocalizations, utilizing the ESC-50 dataset. Our approach involves two distinct methods: Yamnet, a pre-trained deep learning model optimized for sound analysis, and a custom Sequential models (ANN ,RNN , CNN) developed from scratch. The primary motivation for this work lies in addressing real-world applications that require precise sound classification.

## Challenges

The primary challenge we face is the scarcity of labeled data. To overcome this, we explore audio data augmentation techniques, integrating them with our CNN models. Our goal is to achieve state-of-the-art sound classification, bridging the gap between deep learning's potential and real-world problem-solving.

## ESC-50 Dataset

The ESC-50 dataset is a valuable resource for our project. Comprising 2,000 high-quality sound recordings, each categorized into one of 50 distinct classes, it serves as a common choice in the field of sound analysis and machine learning research.

## Custom Model and Data Augmentation

In our project, we address the challenge of classifying cat and dog vocalizations with a custom model optimized for limited data availability. To mitigate data scarcity, we adopt a robust data augmentation strategy, including:

- Time Stretching (TS): Alters the audio speed while preserving pitch .
- Pitch Shifting (PS1): Changes pitch without duration alteration .
- Pitch Shifting (PS2): A second set of pitch shifts with larger values .

This multifaceted augmentation strategy equips our model to handle data limitations, enhancing its adaptability and precision in the classification of cat and dog vocalizations, even in real-world, noisy conditions.


# Claws and Paws Sound-Based Pet Identification

## Model Training and Evaluation

### Artificial Neural Network (ANN) Model

| Epoch | Training Loss | Training Accuracy | Validation Loss | Validation Accuracy |
|-------|---------------|-------------------|------------------|----------------------|
| 1     | 4.6488        | 0.5268            | 4.3846           | 0.5000               |
| ...   | ...           | ...               | ...              | ...                  |
| 40    | 0.1643        | 0.9375            | 0.5425           | 0.7500               |

**Total training time:** 3.71 seconds

### Recurrent Neural Network (RNN) Model

| Epoch | Training Loss | Training Accuracy | Validation Loss | Validation Accuracy |
|-------|---------------|-------------------|------------------|----------------------|
| 1     | 0.6892        | 0.4911            | 0.6721           | 0.3750               |
| ...   | ...           | ...               | ...              | ...                  |
| 40    | 0.2026        | 0.9018            | 0.0287           | 1.0000               |

**Total training time:** 15.40 seconds

### YAMNET Model

| Epoch | Training Loss | Training Accuracy | Validation Loss | Validation Accuracy |
|-------|---------------|-------------------|------------------|----------------------|
| 1     | 0.7997        | 0.5625            | 1.7028           | 0.5000               |
| ...   | ...           | ...               | ...              | ...                  |
| 10    | 0.1691        | 0.9688            | 4.7585           | 0.8125               |

**Total training time:** 3.71 seconds

### Convolutional Neural Network (CNN) Model

| Epoch | Training Loss | Training Recall | Training Precision | Validation Loss | Validation Recall | Validation Precision |
|-------|---------------|------------------|--------------------|------------------|---------------------|-----------------------|
| 1     | 15.8019       | 0.7059           | 0.6857             | 1.6755           | 0.9333              | 0.8235                |
| ...   | ...           | ...              | ...                | ...              | ...                 | ...                   |
| 4     | 0.4414        | 0.9231           | 0.9231             | 0.2029           | 0.9231              | 1.0000                |
**Total training time:** 17 seconds

## Conclusion

After training and evaluating multiple machine learning models for sound classification, we can draw the following conclusions:

- **Artificial Neural Network (ANN):** Competitive performance, further analysis needed for complexity and interpretability.
  
- **Recurrent Neural Network (RNN):** Promising results with a test accuracy of 93.75%. Longer training time (15.40 seconds).

- **YAMNET Model:** Achieves 81.25% validation accuracy with a total training time of 3.71 seconds.

- **Convolutional Neural Network (CNN):** Best-performing model with high accuracy and precision. However, resource-intensive due to a large number of parameters (111,352,605 or 424.78 MB).


## Conclusion

Our project not only contributes to the field of sound analysis but also offers practical solutions for pet owners, animal shelters, veterinarians.

