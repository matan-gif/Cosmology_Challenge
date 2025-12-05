# Starting Kit and Sample Submission
***


## Phase 2: Out-of-Distribution Detection
### Starting Kits
We are preparing starting kits to help participants get started with the competition, understand the data, and prepare submissions for Codabench. 
<!-- You can check the starting kit notebooks on our GitHub repository or through the Google Colab below: -->

<!-- 1. [<ins>**Power Spectrum Analysis**</ins>]() 

    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]()

2. [<ins>**Convolutional Neural Network + MCMC**</ins>]() 

    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]() -->

<!-- 2. [<ins>**Convolutional Neural Network + MCMC**</ins>](https://github.com/FAIR-Universe/Cosmology_Challenge/blob/master/Phase_1_Startingkit_WL_CNN_MCMC.ipynb) 

    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/FAIR-Universe/Cosmology_Challenge/blob/master/Phase_1_Startingkit_WL_CNN_MCMC.ipynb) -->


<!-- #### ⚠️ Note:
- To run the starting kits locally on your device, please directly clone this repository. The `input_data` directory of this repository contains a downsampled dataset that allows you to run the starting kit with minimal efforts. 
- To run the CNN baseline method locally on your device, please make sure that you have installed all required libraries and relevant dependencies. Fore more information, please check our [<ins>**conda instructions**</ins>](https://github.com/FAIR-Universe/Cosmology_Challenge/tree/master/conda).
- To fully train the baseline model and generate a dummy submission that can be scored on our competition website, you will need to download the public training data and the Phase 2 test data from the `Data` tab. The dataset will be publicly available soon.   -->
<!-- or from [**<ins>here</ins>**](https://www.codabench.org/datasets/download/c99c803a-450a-4e51-b5dc-133686258428/). -->



### Dummy Sample Submission
Dummy sample submission is provided for you to understand what is expected as a submission. The sample submission is a zip that only contains one json file named `result.json`. This file contains a list of `InD_prob`. The list contains 6,000 probabilities that each test sample is in-distribution under the training data’s systematics and nuisance-parameter ranges. The probabilities must be values between 0 and 1.

The format looks like this:

```json
{
    "InD_prob": [
            0.8356,
            0.3141
        ... # total 6,000 items
        ]
}
```

<!-- ### ⬇️ [<ins>Dummy Sample Submission</ins>]() -->

<!-- ### ⬇️ [<ins>Dummy Sample Submission</ins>](https://www.codabench.org/datasets/download/65bc826a-a635-4fe5-a20e-89efa8533ad8/) -->
