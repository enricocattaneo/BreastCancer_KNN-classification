# BreastCancer_KNN-classification
Using the Breast Cancer Wisconsin (Diagnostic) Database to create a k-nearest neighbors classifier that can help diagnose patients.


╒═════════════════════╤══════════════╤═════════════╤═════════════╤══════════════════════════════════════════════════════════════════════════════╕
│                     │   Train Acc. │   Test Acc. │   Test Rec. │ Best Model                                                                   │
╞═════════════════════╪══════════════╪═════════════╪═════════════╪══════════════════════════════════════════════════════════════════════════════╡
│ KNN                 │     0.936264 │    0.964912 │    0.93617  │ KNeighborsClassifier(n_neighbors=13)                                         │
├─────────────────────┼──────────────┼─────────────┼─────────────┼──────────────────────────────────────────────────────────────────────────────┤
│ NAIVE BAYES         │     0.945055 │    0.929825 │    0.914894 │ GaussianNB(var_smoothing=1.519911082952933e-09)                              │
├─────────────────────┼──────────────┼─────────────┼─────────────┼──────────────────────────────────────────────────────────────────────────────┤
│ LOGISTIC REGRESSION │     0.96044  │    0.982456 │    1        │ LogisticRegression(C=100, max_iter=5000, solver='newton-cg')                 │
├─────────────────────┼──────────────┼─────────────┼─────────────┼──────────────────────────────────────────────────────────────────────────────┤
│ DECISION TREE       │     0.92967  │    0.921053 │    0.914894 │ DecisionTreeClassifier(criterion='entropy', max_depth=7, random_state=14)    │
├─────────────────────┼──────────────┼─────────────┼─────────────┼──────────────────────────────────────────────────────────────────────────────┤
│ RANDOM FORESTS      │     0.953846 │    0.964912 │    0.957447 │ RandomForestClassifier(max_depth=5, min_samples_leaf=4, min_samples_split=7, │
│                     │              │             │             │                        random_state=14)                                      │
├─────────────────────┼──────────────┼─────────────┼─────────────┼──────────────────────────────────────────────────────────────────────────────┤
│ ADABOOST            │     0.971429 │    0.973684 │    0.957447 │ AdaBoostClassifier(learning_rate=0.01, n_estimators=2000)                    │
├─────────────────────┼──────────────┼─────────────┼─────────────┼──────────────────────────────────────────────────────────────────────────────┤
│ GRADIENT BOOSTING   │     0.971429 │    0.982456 │    0.957447 │ GradientBoostingClassifier(learning_rate=1, max_depth=1, n_estimators=500)   │
├─────────────────────┼──────────────┼─────────────┼─────────────┼──────────────────────────────────────────────────────────────────────────────┤
│ NEURAL NETWORK      │     0.951648 │    0.938596 │    0.93617  │ MLPClassifier(activation='logistic', alpha=0.001, hidden_layer_sizes=25,     │
│                     │              │             │             │               learning_rate='adaptive', max_iter=10000)                      │
╘═════════════════════╧══════════════╧═════════════╧═════════════╧══════════════════════════════════════════════════════════════════════════════╛
