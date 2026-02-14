# FAIR Universe - Weak Lensing ML Uncertainty Challenge (Phase 2)
*** 
This **Phase 2** of Weak Lensing Machine Learning Uncertainty Challenge explores ***out-of-distribution (OoD) detection*** AI techniques for **Weak Gravitational Lensing Cosmology**.

🏗️ The competition will start soon! **You can register now through your affiliation/company email address, and you will receive a notification when it officially start!**  
<!-- 🚀 **Phase 2** of the competition will start soon!  
🚩 To enter the competition, please register through your **affiliation/institutional email**.  -->
***

<!-- <span style="background: linear-gradient(to right, #d0e8ff, #b3d1ff); color: #003366; padding: 24px 36px; border-radius: 8px; font-weight: 600; font-size: 22px; display: inline-block;">
  Phase-2 Leaderboard is <a href="https://fair-universe.lbl.gov/WeakLensing-Uncertainty-Challenge.html" target="_blank" style="color: #0056b3; text-decoration: underline;">here</a>
</span> -->


## Introduction
The large-scale structure of the universe—the cosmic web of galaxies, galaxy clusters, and dark matter spanning hundreds of millions of light-years—encodes essential information about the composition, evolution, and fundamental laws governing the cosmos. However, the majority of matter in the universe is dark matter, which does not interact with light and can only be observed indirectly through its gravitational effects. According to Einstein’s theory of general relativity, the gravitational field of this large-scale structure bends the path of light traveling through the universe. **Weak gravitational lensing** refers to the subtle, coherent distortions in the observed shapes of distant galaxies caused by the deflection of light as it traverses the inhomogeneous matter distribution of the universe. By statistically analyzing these distortions across large regions of the sky, weak lensing provides a powerful probe of the matter distribution and the underlying cosmological model that governs the expansion of the universe.

Traditional analysis based on two-point correlation functions can only capture limited amount of information from the weak lensing data (2D fields similar to images). To fully exploit the non-Gaussian features present in the cosmic web, higher-order statistics and modern machine learning (ML) methods have become increasingly important. These approaches, including deep learning and simulation-based inference, have been shown to extract significant more information in weak lensing maps than traditional techniques. However, different analyses assume different dataset setups and lead to different results, making it hard to directly compare with existing approaches. Furthermore, most (if not all) of these methods rely heavily on simulations that may not accurately represent real data due to modeling approximations and missing systematics. We can frame this problem as an **out-of-distribution (OoD) detection task**; that is, *whether or not the actual observations deviate from the simulation or forward model used to train our models?*

This competition is motivated by the need to quantify and compare the information content that different analysis methods—ranging from classical statistics to ML-based models—can extract from weak lensing maps, while also evaluating their robustness to simulation inaccuracies and observational systematic uncertaintes.

The outcomes of this competition are expected to guide the development of next-generation weak lensing analysis pipelines, foster cross-disciplinary collaboration between the astrophysics and machine learning communities, and ultimately improve the reliability of cosmological inference from current and upcoming surveys such as LSST, Euclid, and the Roman Space Telescope. By explicitly addressing simulation-model mismatch and the need to quantify systematic uncertainties, this competition emphasizes scientific robustness and interpretability, aligning with the growing emphasis on trustworthy ML in scientific domains.


## Competition Tasks: Out-of-Distribution Detection
***
Through this competition, participants will analyze a suite of carefully designed mock weak lensing maps with known cosmological parameters, constructed to include variations in simulation fidelity and several observational systematic uncertainties. By comparing the performance and robustness of different methods in a controlled setting, the competition aims to systematically assess their ability to extract cosmological information while quantifying their sensitivity to modeling assumptions and systematics.

In practice, the participants will be provided with a large labeled training dataset ($\sim$ 26k) to train models that learn useful features for cosmological inference on two key parameters:
- $\Omega_m$: a parameter that represents the fraction of the matter energy density in the universe.
- $S_8$: a parameter that quantifies the amplitude of matter fluctuations in the present-day universe.

Participants have to develop methods for out-of-distribution (OoD) detection, with the goal of identifying a fraction of the test data that deviates from the training distribution through a small $p$-value. 
<!-- The InD probability of an instance of the data can be potentially obtained by, for example, estimating the probability distribution of training data or evaluating some distance metrics between test and training data in a learned feature space. -->

Our training datasets incorporate all major known systematics and are constructed to be as realistic as possible. As a result, we anticipate that models developed through this competition will be directly applicable to real observational data, enabling more robust and precise cosmological measurements.

***
There are several materials regarding the FAIR Universe - Weak Lensing ML Uncertainty Challenge:

* **<ins>Training Data / Test Data</ins>**: Will be available soon.

<!-- * [**<ins>Training Data / Phase 2 Test Data (6.7 GB)</ins>**](https://www.codabench.org/datasets/download/c99c803a-450a-4e51-b5dc-133686258428/): 
The file includes the training data, labels, and the Phase 2 test data for this competition.  -->

* [**<ins>Competition Overview</ins>**](https://fair-universe.lbl.gov/tutorials/WL_Competition_Overview.pdf): This file presents high-level overview about this competition, the train/test data structure, evaluation metrics, and the expected competition timeline.

<!-- * [**<ins>GitHub Repository</ins>**](https://github.com/FAIR-Universe/Cosmology_Challenge/tree/master): This repository hosts the code for testing submissions, as well as the starting kit notebooks ([<ins>Power Spectrum Analysis</ins>](https://github.com/FAIR-Universe/Cosmology_Challenge/blob/master/Phase_2_Startingkit_WL_PSAnalysis.ipynb) , [<ins>Convolutional Neural Network + MCMC</ins>](https://github.com/FAIR-Universe/Cosmology_Challenge/blob/master/Phase_2_Startingkit_WL_CNN_MCMC.ipynb)). The Phase 2 starting kits are also available over the `Starting Kit` tab of this competition or on Google Colab. -->


## How to join this competition?
***
- Login or Create Account on [<ins>Codabench</ins>](https://www.codabench.org/) 

   🚩 **Please register through your affiliation/company email address.** Contact us if you have any problems with this.

  🏗️  **The competition will start soon. Registering now so that you will be notified when the competition start.**  

- After the competition starts, go to the `Starting Kit` tab
- Download the `Dummy Sample Submission`
- Go to the `My Submissions` tab
- Register in the Competition
- Submit the downloaded file


## Submissions
***
This competition allows only result submissions. Participants can submit a result submission as instructed in the `Starting Kit` tab.


## Timeline
***
Available soon.
<!-- ![alt text](image-2.png) -->

## Credits
***
#### Institute for Advanced Study
- Biwei Dai 

#### Lawrence Berkeley National Laboratory
- Wahid Bhimji
- Paolo Calafiura
- Po-Wen Chang
- Sascha Diefenbacher
- Steven Farrell
- Chris Harris

#### University of California, Berkeley
- Jordan Dudley
- Uroš Seljak

#### Stanford University / SLAC National Accelerator Laboratory
- Benjamin Nachman

#### University of Washington
- Yuan-Tang Chou
- Elham E Khoda
- Yulei Zhang

#### ChaLearn
- Isabelle Guyon
- Ihsan Ullah

#### Université Paris-Saclay
- Ragansu Chakkappai
- David Rousseau

#### University of Toronto
- Ibrahim Elsharkawy



## Contact
***
Visit our website: <ins>https://fair-universe.lbl.gov/</ins>

Email: <ins>fair-universe@lbl.gov</ins>

Updates will be announced through the [<ins>Codabench forum</ins>](https://www.codabench.org/forums/8787/).