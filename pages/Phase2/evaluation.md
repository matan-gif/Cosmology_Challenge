# Evaluation
***
Participants must submit their predictions to the Codabench platform using the test data we provide. 

- ### Phase 2: Out-of-Distribution Detection

    The Phase-2 test data will contain 10,000 instances (2D fields similar to images), with some instances generated assuming different physical models (OoD). The OoD test samples are labeled by $y_i=0$, while InD test samples are labeled by $y_i=1$. Participants will not be provided with the ground truth labels, any OoD examples, or any information on how the OoD test data are generated. 

    Given any test sample $i$, participant's model should determine a $p$-value $\hat{p}_i$ using any test statistics that can be predicted by the model. The $p$-value is the probability of observing a test statistic $TS$ *at least as extreme as* what is obtained from the test sample, assuming the test sample is InD
        $$
            \hat{p}_i = \text{probability}~(TS_{\rm InD} \text{ is more extreme than } TS_{i}) \in [0, 1]~.
        $$
    Under this definition, smaller $\hat{p}_i$ indicates greater inconsistency with the InD distribution; therefore, it can be regarded as a sort of InD score, and one can choose a threshold $p_{\rm th}$ of the $p$-value below which the test samples are detected as OoD; otherwis, detected as InD.

    In this challenge, the model's OoD detection performance will then be evaluated with the area under the ROC (Receiver Operating Characteristic) curve defined by the True Positive Rate as a function of the False Positive Rate over a range of the $p$-value thresholds
        $$
            \text{Phase-2 score} \equiv \text{Area under ROC}~(0.005 \leq p_{\rm th} \leq 0.05)~. 
        $$

    We will provide the Phase-2 test data when the Phase 2 starts.


<!-- - ### Phase 2: Out-of-Distribution Detection
    Participants' models should determine the **in-distribution probability $\hat{p}_{{\rm InD}, i}$** that the given dataset is consistent with the training data. The model's OoD detection performance will be assessed with the following score
        $$
            \textrm{score}_{\textrm{OoD}} = \frac{1}{N_{test}} \sum_{i}^{N_{\rm test}} \left[y_i \log(\hat{p}_{{\rm InD}, i}+ \epsilon)+(1-y_i)\log(1-\hat{p}_{{\rm InD}, i} + \epsilon)\right]~, 
        $$
    where $\hat{p}_{{\rm InD},i} \in [0, 1]$, $y_i=1$ if the dataset is InD, $y_i=0$ if the dataset is OoD, and $\epsilon$ is a small positive constant to avoid a score of $-\infty$. 
    

    The Phase 2 test data will contain 6,000 instances (2D fields similar to images), with some instances generated assuming different physical models (OoD). The participants' models should estimate the probability $p_i$ of whether each test data is drawn from the same distribution as the training data. The participant will not be provided with OoD examples or any information on how the OoD test data are generated. 

    We will provide the Phase 2 test data when the Phase 2 starts. -->