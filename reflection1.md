# Data Science Reflection 1
## Machine Learning and Epileptic Seizures

In the past, electroencephalograms (EEGs) have been used to perform a multitude of medical tests to help determine abnormalities in brain function. The data science method of machine learning has also been used in medicine to aide in cancer diagnoses and “interpret electronic health records” (Roy et al., 2019). A recent study from Cornell has shown that the two can be combined to help improve the quality of healthcare for epilepsy patients. The scientists involved were hoping to use AI to not only have automatic detection of seizures, but also automatically classify seizure types as they occur. They used the Temple University Hospital (TUH) EEG Seizure Corpus to run this experiment on seizure types and utilized preprocessing techniques and machine learning algorithms. 

The first step for this study was pre-processing. Pre-processing data consists of cleaning, normalizing, and transforming raw data into information that can be utilized for scientific research. Two methods for manipulating the data were used, both of which started with Fast Fourier Transformation. FFT is an algorithm that converts data from its original format to one that represents the frequency domain (Roy et al., 2019). Method one (v1.4.0) took the FFT data and then took the Log10 values (Roy et al., 2019). Method two (v1.5.2) took the FFT data as well, but then clipped from 1 to fmax Hz and normalized frequency buckets (Roy et al., 2019). The difference between these two methods is that method one had 5 cross validation folds and method 2 only had 3, which created differing data as shown in the chart below. It was mainly just differing patient numbers and averages which led to differing data. There were also different classification algorithms used to analyze the data. Researchers used K-Nearest Neighbors (k-NN), Stochastic Gradient Descent (SGD), XGBoost, and Convolutional Neural Networks (CNN) (Roy et al., 2019). ![seizuretype](C:\Users\MAC4r\Downloads\rstudio_datascience\seizuretype.png)

In addition, machine learning was used throughout the entire study and was the main data science method utilized by the researchers. The researchers were using “specialized neural networks to classify EEG data into normal/abnormal EEG” tests to start classifying seizure types (Roy et al., 2019). Using the pre-processing and statistical analysis of the data, machine learning could become more effective in recognizing seizure types. By improving the technology that can distinguish between seizure types, seizures can be recorded and automatically uploaded to digital diaries for patients, which will in turn improve the quality of healthcare available for patients. 

These advancements are so important to the healthcare field for multiple reasons. First, 1% of the world has epilepsy, and 2/3 of this population has no treatment available for them due to inconsistencies in how epilepsy is tracked and diagnosed (Roy et al., 2019). In fact, the main way of managing epilepsy is through trial and error or manual diaries on the patients end, which is only reliable half of the time (Roy et al., 2019). Patients that suffer from any of the seizure types that were analyzed in this study (FNSZ, GNSZ, SPSZ, CPSZ, ABSZ, TNSZ, TCSZ, MYSZ) have the ability to streamline the diagnosis and treatment process with the use of their cellphone (Roy et al., 2019). The implications of this study could completely revolutionize this section of healthcare, and dramatically improve the quality of life for millions of people worldwide. Not only can it help with epilepsy, but the machine learning and EEG combination could benefit other neurological disorders, such as dementia and various sleep disorders. 

 ![eegseizure](C:\Users\MAC4r\Downloads\rstudio_datascience\eegseizure.jpg)

The image above is an example of EEG readings on a patient with epilepsy (Wang, Long, Arends, & Aarts, 2017).



Roy, S., Asif, U., Tang, J., & Harrer, S. (2019). Machine learning for seizure type classification: 

setting the benchmark. *arXiv* *preprint arXiv:1902.01012*. 

Wang, L., Long, X., Arends, J., & Aarts, R. (2017). [EEG scan of seizure activity]. Retrieved September 10, 2020, from https://doi.org/10.1016/j.jneumeth.2017.07.013 

