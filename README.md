<h1 align="center">Tweet Sentiment Analysis</h1>

<br/>

<h2>📝 <strong>Description</strong></h2>
<p>
This project focuses on identifying and analyzing the sentiments expressed in Turkish tweets from 2022. The aim is to raise awareness about individuals expressing grief, pain, and loneliness on social media. By retrieving tweets via the Twitter API and excluding content unrelated to emotions (e.g., politics, news), the dataset emphasizes personal feelings. Tweets were manually labeled based on the sentiment they conveyed. A Logistic Regression model was developed to analyze live tweets and interact with users posting negatively tagged tweets by suggesting motivational playlists.
</p>

<h2>📂 <strong>Dataset</strong></h2>
<ul>
  <li><strong>tweets_labeled.csv:</strong> Contains 12,690 observations with tweet content, timestamps, and sentiment labels (-1: Negative, 0: Neutral, 1: Positive).</li>
  <li><strong>tweets_21.csv:</strong> Contains 13,272 observations of tweets from 2021.</li>
</ul>
<p><em>Dataset available on <a href="https://www.kaggle.com/datasets/vedatgul/nlp-tweets" target="_blank">Kaggle</a>.</em></p>


<h3>Dataset Variables</h3>
<ul>
  <li><strong>tweet_id:</strong> Unique identifier for each tweet.</li>
  <li><strong>tweet:</strong> The content of the tweet.</li>
  <li><strong>date:</strong> Timestamp of the tweet.</li>
  <li><strong>label:</strong> Sentiment label (-1, 0, 1).</li>
</ul>

<h2>🛠️ <strong>Feature Engineering</strong></h2>
<p>
Key preprocessing steps include:
</p>
<ul>
  <li>Handling missing values by removing rows with null data.</li>
  <li>Converting timestamps to the <strong>Europe/Istanbul</strong> timezone.</li>
  <li>Creating new time-based variables like <strong>season</strong>, <strong>day</strong>, and <strong>period</strong> from the timestamp.</li>
  <li>Cleaning tweets by removing emojis and special characters using regex.</li>
</ul>

<h3>🔍 Analysis of Target Variable</h3>
<p>
Detailed exploration of the dataset revealed patterns like:
</p>
<ul>
  <li><strong>Distribution of Negative Tweets:</strong> Analyzed based on weekdays, dates, and tweet content.</li>
  <li><strong>Common Themes:</strong> Highlighted frequently occurring expressions in negative tweets.</li>
</ul>

<h2>🤖 <strong>Modeling</strong></h2>
<h3>Logistic Regression</h3>
<ul>
  <li>Used <strong>TF-IDF Vectorization</strong> to transform text data into numerical representations.</li>
  <li>Split data into training and testing sets for model evaluation.</li>
  <li>Trained a Logistic Regression model with an increased max_iter value for convergence.</li>
</ul>

<h3>Model Evaluation</h3>
<ul>
  <li><strong>Accuracy:</strong> The model achieved an accuracy of <strong>~79.4%</strong>.</li>
  <li><strong>Debug Information:</strong> Verified data shapes and predicted values for consistency.</li>
</ul>

<h2>❗ <strong>Key Note</strong></h2>
<p>
The code uses the Python convention of <code>if __name__ == "__main__":</code>, ensuring that the main function is executed only when the script is run directly, not when imported as a module. This structure keeps the reusable components separate from the primary execution logic.
</p>

<h2>📊 <strong>Conclusion</strong></h2>
<p>
The sentiment analysis model effectively classifies tweets, with an accuracy of 79.4%, showcasing its potential to identify and respond to users expressing negative emotions. This tool highlights how machine learning can be applied to social media analytics for meaningful interventions.
</p>

<h2>🔧 <strong>Technologies Used</strong></h2>
<div align="center">
    <img src="https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" alt="Python"/>
    <img src="https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas"/>
    <img src="https://img.shields.io/badge/numpy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy"/>
    <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" alt="Scikit-learn"/>
    <img src="https://img.shields.io/badge/matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white" alt="Matplotlib"/>
</div>

<h2>📢 <strong>Contact</strong></h2>
<ul>
  <li><a href="https://www.linkedin.com/in/yourusername/" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white" alt="LinkedIn"/></a></li>
  <li><a href="mailto:your.email@example.com"><img src="https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white" alt="Email"/></a></li>
</ul>

<p align="center">&copy; 2025 Your Name. All rights reserved.</p>

<hr/>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=ecembayindir&repo=Natural-Language-Processing-Tweet-Sentiments&label=Repository%20views&color=0e75b6&style=flat" alt="Repository Views">
</p>
