# BU_DM_Project
**Classification model to predict hospital mortality among heart failure patients at beth israel hospital in Boston, MA**

This term project aims to predict hospital mortality from a sample data of 1177 patients who suffered from heart failure. Therefore, a binary label is estimated, indicating whether an individual may be more likely to survive or perish during the treatment process. The variables used for this classification task consist of demographic patient records, such as age, gender, and medical data collected from blood and urine samples.

In order to build an accurate classification model, this applied research project follows the standard data mining procedure. First, the patient records are examined during an initial data exploration phase which helps us identify any correlations between the features and target class. This supports the machine learning process, as these valuable attributes can largely explain the variance of the class attribute. Furthermore, it may prevent the model from over-fitting, given a large number of available attributes (47 to be exact). In order to overcome this issue, several feature selection methods are used to generate subsets of attributes that help the model to predict the hospital mortality accurately. The data subsets generated during this step are then used to train and test the following five classification models: Logistic Regression, Gaussian Naïve Bayes, Decision Tree, Random Forest, and Gradient Boost. Finally, the performance of these estimators is evaluated using a set of standard metrics such as precision, recall, and accuracy. In order to obtain rigorous results, the models are additionally trained using the “10-Fold cross-validation” method. From a technical perspective, the project is implemented using the Python library “sci-kit learn.” The data pre-processing and feature selection steps are implemented using pipelines. Furthermore, it also contains a processing step of randomized over-sampling, given the imbalanced target attribute in the dataset.

The performance results of the 25 generated model instances indicates that classification accuracy of up to 89% can be achieved using random forest classification. However, the metrics also disclose that this model type has a particularly strong precision while showing a weak recall rate. Since mistaking a patient with low survival chances for a patient with good conditions can be understood as an ethical dilemma, due to this, the authors put more weight on recall. Consequently, the Gaussian Naïve Bayes classifier is found to be the best fit for the purpose, showing a recall rate of 78% and an overall accuracy of 81%. The selected features that contribute to this accuracy were 'Urine output', 'Leucocyte', 'Urea nitrogen', 'Blood calcium', 'Anion gap', and 'Bicarbonate'.

**Acknowledgments:** Zhou, Jingmin, Li, Fuhai, Song, Yu, Fu, Mingqiang, Han, Xueting, & Ge, Junbo. (2021). Prediction model of in-hospital mortality in intensive care unit patients with heart failure: Machine learning-based, retrospective analysis of the MIMIC-III database. 
**Data Source:** https://doi.org/10.5281/ZENODO.5032847
