# Binary Classification with a Software Defects👾
<h3>Problem Statement📌</h3>
The given dataset was dataset from competition on Kaggle which is generated from a deep learning model trained on the Software Defect Dataset. And we need to predicts defects in C programs given various various attributes about the code.
<br> <h3> Data Description📑</h3>
about the features we have 22 features
<li> loc: numeric - McCabe's line count of code </li>
<li>v(g): numeric - McCabe "cyclomatic complexity"</li>
<li>ev(g): numeric - McCabe "essential complexity"</li>
<li>iv(g): numeric - McCabe "design complexity"</li>
<li>n: numeric - Halstead total operators + operands</li>
<li>v: numeric - Halstead "volume"</li>
<li>l: numeric - Halstead "program length" </li>
<li>d: numeric - Halstead "difficulty"</li>
<li>i: numeric - Halstead "intelligence"</li>
<li>e: numeric - Halstead "effort"</li>
<li>b: numeric - Halstead</li>
<li>t: numeric - Halstead's time estimator</li>
<li>lOCode: numeric - Halstead's line count</li>
<li>lOComment: numeric - Halstead's count of lines of comments</li>
<li>lOBlank: numeric - Halstead's count of blank lines</li>
<li>lOCodeAndComment: numeric</li>
<li>uniq_Op: numeric - unique operators</li>
<li>uniq_Opnd: numeric - unique operands</li>
<li>total_Op: numeric - total operators</li>
<li>total_Opnd: numeric - total operands</li>
<li>branchCount: numeric - percentage of the flow graph</li>
<li>defects: {false, true} - module has/has not one or more reported defects</li>
<h3>Our Processes🔍</h3>
<li>Loading Libraries</li>
<li>Reading Data Files</li>
<li>Data Exploration</li>
<li>Data Preparation</li>
<li>Data Modeling</li>
<li>Model Evaluation</li>
<h3>And we got this❣️</h3>

| Version<br>Number | Version Details | Model Using|Public LB Score|
| :-: | --- | :-: | :-: |
| **V1** |- Log Transformation, Standard Scaler, PCA<br> - No new features <br> - LGC, XGBoost, HGBC, KNN, ExtraTree <br> |Ensemble(ExtraTree,HGBC,XGBoost) |0.49|
| **V2** |- No Normalization<br> - Put PCA, Standard Scaler into pipeline <br> - No new features <br> - Same algorithm as V1 |Ensemble(ExtraTree,HGBC,XGBoost) |0.78922|
| **V3** |- Add Robust Scaler <br> - create function to Prepare every each dataset for model <br> - Put PCA, Standard Scaler into pipeline <br> - Same algorithm as V1  |Ensemble(ExtraTree,HGBC,XGBoost)|0.78986|

<h3>for more details about my project you can see in <a href="https://www.kaggle.com/code/sirintornphachai/dsi311-binary-classification/notebook">this</a>😊🎉</h3>
