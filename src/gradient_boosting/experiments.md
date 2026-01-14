# Experiment: 0
> Initial configuration
- **Date:** 2026-01-14 20:30:54
- **Mean AUC:** `0.5481 +/- 0.0256`
- **Threshold:** `0.5`

## Model Configuration
```python
LGBMClassifier(learning_rate=0.05, objective='binary', random_state=1,
               scale_pos_weight=5, verbosity=1)
```

## Fold Results
### Fold 1
- **Fold AUC:** `0.5893`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9990 | 0.9959 | 0.9974 |
| 1 | 0.0525 | 0.1828 | 0.0815 |

#### Confusion Matrix Fold 1
![CM Fold 1](../../images/gbdt/0/cm_fold_1.jpg)

---
### Fold 2
- **Fold AUC:** `0.5096`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9989 | 0.9957 | 0.9973 |
| 1 | 0.0060 | 0.0235 | 0.0096 |

#### Confusion Matrix Fold 2
![CM Fold 2](../../images/gbdt/0/cm_fold_2.jpg)

---
### Fold 3
- **Fold AUC:** `0.5536`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9992 | 0.9960 | 0.9976 |
| 1 | 0.0251 | 0.1111 | 0.0409 |

#### Confusion Matrix Fold 3
![CM Fold 3](../../images/gbdt/0/cm_fold_3.jpg)

---
### Fold 4
- **Fold AUC:** `0.5402`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9992 | 0.9950 | 0.9971 |
| 1 | 0.0141 | 0.0854 | 0.0241 |

#### Confusion Matrix Fold 4
![CM Fold 4](../../images/gbdt/0/cm_fold_4.jpg)

---
### Fold 5
- **Fold AUC:** `0.5480`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9992 | 0.9961 | 0.9977 |
| 1 | 0.0211 | 0.1000 | 0.0348 |

#### Confusion Matrix Fold 5
![CM Fold 5](../../images/gbdt/0/cm_fold_5.jpg)

---


# Experiment: 1
> Applied RandomUnderSampler
- **Date:** 2026-01-14 20:32:56
- **Mean AUC:** `0.6621 +/- 0.0119`
- **Threshold:** `0.5`

## Model Configuration
```python
Pipeline(steps=[('sampler',
                 RandomUnderSampler(random_state=1, sampling_strategy=0.01)),
                ('classifier',
                 LGBMClassifier(learning_rate=0.05, objective='binary',
                                random_state=1, scale_pos_weight=5,
                                verbosity=1))])
```

## Fold Results
### Fold 1
- **Fold AUC:** `0.6646`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9992 | 0.9959 | 0.9975 |
| 1 | 0.0923 | 0.3333 | 0.1445 |

#### Confusion Matrix Fold 1
![CM Fold 1](../../images/gbdt/1/cm_fold_1.jpg)

---
### Fold 2
- **Fold AUC:** `0.6502`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9992 | 0.9946 | 0.9969 |
| 1 | 0.0588 | 0.3059 | 0.0987 |

#### Confusion Matrix Fold 2
![CM Fold 2](../../images/gbdt/1/cm_fold_2.jpg)

---
### Fold 3
- **Fold AUC:** `0.6799`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9994 | 0.9947 | 0.9970 |
| 1 | 0.0597 | 0.3651 | 0.1027 |

#### Confusion Matrix Fold 3
![CM Fold 3](../../images/gbdt/1/cm_fold_3.jpg)

---
### Fold 4
- **Fold AUC:** `0.6680`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9994 | 0.9945 | 0.9970 |
| 1 | 0.0490 | 0.3415 | 0.0858 |

#### Confusion Matrix Fold 4
![CM Fold 4](../../images/gbdt/1/cm_fold_4.jpg)

---
### Fold 5
- **Fold AUC:** `0.6478`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9994 | 0.9956 | 0.9975 |
| 1 | 0.0540 | 0.3000 | 0.0915 |

#### Confusion Matrix Fold 5
![CM Fold 5](../../images/gbdt/1/cm_fold_5.jpg)

---


# Experiment: 2
> Increased threshold
- **Date:** 2026-01-14 20:35:11
- **Mean AUC:** `0.6181 +/- 0.0059`
- **Threshold:** `0.7`

## Model Configuration
```python
Pipeline(steps=[('sampler',
                 RandomUnderSampler(random_state=1, sampling_strategy=0.01)),
                ('classifier',
                 LGBMClassifier(learning_rate=0.05, objective='binary',
                                random_state=1, scale_pos_weight=5,
                                verbosity=1))])
```

## Fold Results
### Fold 1
- **Fold AUC:** `0.6226`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9991 | 0.9979 | 0.9985 |
| 1 | 0.1285 | 0.2473 | 0.1691 |

#### Confusion Matrix Fold 1
![CM Fold 1](../../images/gbdt/2/cm_fold_1.jpg)

---
### Fold 2
- **Fold AUC:** `0.6105`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9991 | 0.9976 | 0.9984 |
| 1 | 0.0922 | 0.2235 | 0.1306 |

#### Confusion Matrix Fold 2
![CM Fold 2](../../images/gbdt/2/cm_fold_2.jpg)

---
### Fold 3
- **Fold AUC:** `0.6176`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9993 | 0.9971 | 0.9982 |
| 1 | 0.0718 | 0.2381 | 0.1103 |

#### Confusion Matrix Fold 3
![CM Fold 3](../../images/gbdt/2/cm_fold_3.jpg)

---
### Fold 4
- **Fold AUC:** `0.6266`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9994 | 0.9972 | 0.9983 |
| 1 | 0.0695 | 0.2561 | 0.1094 |

#### Confusion Matrix Fold 4
![CM Fold 4](../../images/gbdt/2/cm_fold_4.jpg)

---
### Fold 5
- **Fold AUC:** `0.6133`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9993 | 0.9980 | 0.9987 |
| 1 | 0.0874 | 0.2286 | 0.1265 |

#### Confusion Matrix Fold 5
![CM Fold 5](../../images/gbdt/2/cm_fold_5.jpg)

---


# Experiment: 3
> Changed training data to have 1000 0's and 50 1's
- **Date:** 2026-01-14 21:40:14
- **Mean AUC:** `0.6114 +/- 0.0222`
- **Threshold:** `0.5`

## Model Configuration
```python
LGBMClassifier(learning_rate=0.05, objective='binary', random_state=1,
               scale_pos_weight=5, verbosity=1)
```

## Fold Results
### Fold 1
- **Fold AUC:** `0.5781`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9741 | 0.9895 | 0.9817 |
| 1 | 0.3333 | 0.1667 | 0.2222 |

#### Confusion Matrix Fold 1
![CM Fold 1](../../images/gbdt/3/cm_fold_1.jpg)

---
### Fold 2
- **Fold AUC:** `0.6064`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9718 | 0.9628 | 0.9673 |
| 1 | 0.2000 | 0.2500 | 0.2222 |

#### Confusion Matrix Fold 2
![CM Fold 2](../../images/gbdt/3/cm_fold_2.jpg)

---
### Fold 3
- **Fold AUC:** `0.6308`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9471 | 0.9949 | 0.9704 |
| 1 | 0.8000 | 0.2667 | 0.4000 |

#### Confusion Matrix Fold 3
![CM Fold 3](../../images/gbdt/3/cm_fold_3.jpg)

---
### Fold 4
- **Fold AUC:** `0.6012`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9382 | 0.9882 | 0.9625 |
| 1 | 0.6000 | 0.2143 | 0.3158 |

#### Confusion Matrix Fold 4
![CM Fold 4](../../images/gbdt/3/cm_fold_4.jpg)

---
### Fold 5
- **Fold AUC:** `0.6407`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9784 | 0.9956 | 0.9870 |
| 1 | 0.6667 | 0.2857 | 0.4000 |

#### Confusion Matrix Fold 5
![CM Fold 5](../../images/gbdt/3/cm_fold_5.jpg)

---


# Experiment: 4
> scale_pos_weight 5 -> 2, train set 6000 benign, 300 malignant, folds 5 -> 3
- **Date:** 2026-01-14 21:44:38
- **Mean AUC:** `0.7074 +/- 0.0340`
- **Threshold:** `0.5`

## Model Configuration
```python
LGBMClassifier(learning_rate=0.05, objective='binary', random_state=1,
               scale_pos_weight=2, verbosity=1)
```

## Fold Results
### Fold 1
- **Fold AUC:** `0.6633`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9602 | 0.9965 | 0.9780 |
| 1 | 0.8537 | 0.3302 | 0.4762 |

#### Confusion Matrix Fold 1
![CM Fold 1](../../images/gbdt/4/cm_fold_1.jpg)

---
### Fold 2
- **Fold AUC:** `0.7127`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9693 | 0.9930 | 0.9810 |
| 1 | 0.7742 | 0.4324 | 0.5549 |

#### Confusion Matrix Fold 2
![CM Fold 2](../../images/gbdt/4/cm_fold_2.jpg)

---
### Fold 3
- **Fold AUC:** `0.7462`

| Class | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- |
| 0 | 0.9821 | 0.9864 | 0.9842 |
| 1 | 0.5753 | 0.5060 | 0.5385 |

#### Confusion Matrix Fold 3
![CM Fold 3](../../images/gbdt/4/cm_fold_3.jpg)

---


