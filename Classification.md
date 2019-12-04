## classification_report pour x uniquement
```
precision    recall  f1-score   support

        bike       0.86      0.92      0.89       418
         sit       0.98      0.98      0.98       500
  stairsdown       0.78      0.51      0.61       380
    stairsup       0.71      0.82      0.76       402
       stand       0.97      0.94      0.96       466
        walk       0.84      0.94      0.89       505

    accuracy                           0.87      2671
   macro avg       0.86      0.85      0.85      2671
weighted avg       0.87      0.87      0.86      2671
```

## classification_report pour x,y,z
```
              precision    recall  f1-score   support

        bike       0.92      0.95      0.94       418
         sit       1.00      0.99      0.99       500
  stairsdown       0.89      0.79      0.84       380
    stairsup       0.82      0.89      0.85       402
       stand       0.99      0.98      0.98       466
        walk       0.94      0.93      0.94       505

    accuracy                           0.93      2671
   macro avg       0.93      0.92      0.92      2671
weighted avg       0.93      0.93      0.93      2671
```
# avec une normallisation des données x,y,z
## classification_report pour x uniquement
```
              precision    recall  f1-score   support

        bike       0.92      0.82      0.87       409
         sit       1.00      1.00      1.00       505
  stairsdown       0.71      0.58      0.64       367
    stairsup       0.74      0.79      0.76       434
       stand       0.97      0.96      0.97       446
        walk       0.81      0.94      0.87       510

    accuracy                           0.86      2671
   macro avg       0.86      0.85      0.85      2671
weighted avg       0.86      0.86      0.86      2671
```
## classification_report pour x,y,z
```
              precision    recall  f1-score   support

        bike       0.93      0.94      0.93       409
         sit       1.00      1.00      1.00       505
  stairsdown       0.88      0.79      0.83       367
    stairsup       0.82      0.88      0.84       434
       stand       0.99      0.98      0.99       446
        walk       0.94      0.94      0.94       510

    accuracy                           0.93      2671
   macro avg       0.92      0.92      0.92      2671
weighted avg       0.93      0.93      0.93      2671
```
# avec keras
## conv1D
```
              precision    recall  f1-score   support

           0       0.74      0.72      0.73       650
           1       1.00      0.92      0.96      1990
           2       0.87      1.00      0.93       452
           3       0.95      0.80      0.87       370
           4       0.78      0.76      0.77       725
           5       0.92      0.98      0.95      2397

    accuracy                           0.90      6584
   macro avg       0.87      0.86      0.87      6584
weighted avg       0.91      0.90      0.90      6584
```
## conv1D et Unet

```
--- Classification report for test data ---

              precision    recall  f1-score   support

           0       0.74      0.57      0.64     25994
           1       0.99      0.95      0.97     79525
           2       0.90      0.99      0.94     18007
           3       0.99      0.86      0.92     14875
           4       0.72      0.76      0.74     29071
           5       0.90      0.97      0.93     95888

    accuracy                           0.90    263360
   macro avg       0.87      0.85      0.86    263360
weighted avg       0.90      0.90      0.90    263360

```
## conv1D et Vnet

```
--- Classification report for test data ---

              precision    recall  f1-score   support

           0       0.66      0.69      0.68     25994
           1       1.00      0.91      0.95     79525
           2       0.82      0.99      0.90     18007
           3       0.93      0.74      0.83     14875
           4       0.86      0.71      0.78     29071
           5       0.88      0.98      0.93     95888

    accuracy                           0.89    263360
   macro avg       0.86      0.84      0.84    263360
weighted avg       0.89      0.89      0.89    263360
```

## conv1D, windows=180, 20% recovery
```
--- Classification report for test data ---

              precision    recall  f1-score   support

           0       0.83      0.90      0.87       216
           1       1.00      0.96      0.98       664
           2       0.84      0.92      0.88       151
           3       0.89      0.77      0.82       122
           4       0.88      0.87      0.87       244
           5       0.97      0.98      0.98       797

    accuracy                           0.94      2194
   macro avg       0.90      0.90      0.90      2194
weighted avg       0.94      0.94      0.94      2194
```
