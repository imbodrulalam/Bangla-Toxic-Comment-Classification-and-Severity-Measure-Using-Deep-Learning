# Bangla Toxic Comment Classification and Severity Measure Using Deep Learning
## Reference
Haque, Naimul & Alam, Md & Ath Towfiq, Abdullah & Hossain, Mehorab. (2022). Bangla Toxic Comment Classification and Severity Measure Using Deep Learning. Online users nowadays leave a lot of comments on various social networks, news websites, and forums. Certain comments are harmful or abusive. Since it is impractical to manually monitor so many comments, the majority of systems employ some form of a machine learning model to automatically identify harmful content. Much of the work has been done for the English language. However, only a few approaches have been taken to classify toxic comments in the Bangla language. A multi-label classification technique for Bangla comments is offered in the study that follows to classify the numerous toxic comments into six categories: toxic, severe toxic, obscene, threat, insult, and identity hate, and also measure the severity of these comments. For the experiment, we compiled a dataset of 12634 comments from TikTok and other sources. By incorporating knowledge from earlier proposed studies, the proposed classification model was developed utilizing deep learning techniques, specifically Long Short-Term Memory (LSTM) and Long Short-Term Memory-Convolutional Neural Networks (LSTM-CNNs), as well as word embeddings and obtained a maximum accuracy of 83.66% and 1.61 MSE loss for the severity measure.

## Dataset
[[Hugging Face: naimul011/BanglaToxicCommentsDB](https://huggingface.co/datasets/naimul011/BanglaToxicCommentsDB)]([https://link-url-here.org](https://huggingface.co/datasets/naimul011/BanglaToxicCommentsDB))

This repository contains code for detecting and measuring the severity of Bangla toxic comments. The code uses a combination of machine learning techniques to classify comments as toxic or non-toxic and to rate the severity of toxic comments.

## Code Description

The code is written in Python and consists of the following major steps:

1. Importing Libraries: The necessary libraries, including pandas, numpy, matplotlib, seaborn, keras, csv, random, and others, are imported.

2. Loading Datasets: The code loads the Bangla comments dataset from a Google Drive link.

3. Data Analysis and Visualization: The code performs data analysis and visualization to understand the dataset's structure and characteristics. It includes exploring features, checking for missing values, analyzing comment lengths, examining label distribution, and visualizing correlations among different toxic comment categories.

4. Data Pre-processing: The code pre-processes the comment text by removing punctuation, stopwords, and performing stemming using the Bangla stemmer. It also replaces specific strings, such as emojis, with empty strings.

5. Classification of Bangla Toxic Comments: The code uses two different models, LSTM (Long Short-term Memory) and LSTM-CNN (Convolutional Neural Network), to classify Bangla toxic comments. It trains these models using the pre-processed comment data and evaluates their performance using accuracy metrics. It also provides visualizations of the training history, including accuracy and loss plots.

6. Severity Measure of Bangla Toxic Comments: The code calculates the severity score for each comment based on its predicted toxicity. It compares the predicted severity score with the actual severity score available in the dataset. It also provides visualizations, including a histogram of severity scores and a comparison between actual and predicted severity scores.

7. Error Analysis: The code calculates the Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and Mean Absolute Error (MAE) between the actual and predicted severity scores.

## Usage

To use the code, follow these steps:

1. Install the required libraries mentioned in the code (e.g., pandas, numpy, matplotlib, seaborn, keras, etc.).

2. Download the Bangla comments dataset from the provided Google Drive link and save it as `bangla_comments.csv` in the appropriate directory.

3. Run the code step by step, examining the output, visualizations, and model performance metrics.

4. Utilize the trained models to classify new Bangla comments as toxic or non-toxic by using the `rateSeveity()` function to measure the severity of toxic comments.

Note: Make sure to have the necessary dependencies installed and the dataset accessible before running the code.

## License

The code in this repository is licensed under the [MIT License](LICENSE).

## Acknowledgments

The code is based on the work of the original authors and the dataset contributors. Their efforts in collecting the dataset and developing the classification and severity measurement models are greatly appreciated.

## Disclaimer

The code is provided as-is and without any warranty. The authors and contributors shall not be held liable for any damages or losses arising from the use of this code.
