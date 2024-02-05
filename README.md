# Spoken_Language_Identification_Custom_Model


<h2>Introduction</h2>
<p>
The technique that recognizes the language being spoken in an audio recording automatically is known as spoken language identification (SLID), sometimes known as language identification (LID). It's similar to Shazam for languages in that it detects the language based on its acoustic properties rather than the melody of the music. This is an explanation:
<ul>
<li>Audio recording of a spoken word entered.</li>
<li>Output: The recorded language, such as English, Spanish, or French.</li>
</ul>
SLID has a wide range of uses, including
<ul>
<li>Machine translation: Determining the target language for translation is aided by identifying the language of spoken content.</li>
<li>Automatic speech recognition (ASR): Selecting the right ASR system for precise transcription is aided by linguistic knowledge.</li>
<li>Identifying languages for potentially offensive content is known as content moderation.
<li>Putting calls through to customer care representatives who speak the relevant language in many languages.
In this section, we discussed about 3 models for SLID a Custom neural network model  in five languages—English, Tamil, German, French, and Portuguese—is developed, LIDBOX  and Spleechflow open source model.  
</p>

<h2>Custom Model Architecture</h2>


<center>![image](https://github.com/ChayanGhosh1412/Spoken_Language_Identification_Custom_Model/assets/93574637/56595900-8c3d-415c-8df4-faf2d1833562)</center>

By using Deep Neural Networks (DNN), Convolutional Neural Networks (CNN), and Gated Recurrent Unit (GRU), the issues presented by a variety of linguistic situations are intended to be addressed by utilizing the capabilities of these architectures to increase spoken language recognition accuracy. The general architecture of the deep learning models are as follows:
<ol>
  <li><b>Data Collection</b></li>
  <ul>
    <li>The dataset utilized in this study is sourced from <b>Common Voice</b></li>
    <li>Audio files were loaded from the dataset</li>
  </ul>

  <li><b>Feature Extraction</b></li>
    <ul>
    <li>MFCC (Mel-Frequency Cepstral Coefficients) features were extracted from the audio files using the Librosa library.</li>
    <li>MFCCs are effective in capturing key characteristics of speech signals</li>
  </ul>
  
  <li><b>Data Processing</b></li>
   <ul>
    <li>Extracted MFCCs and corresponding language labels were converted into NumPy arrays for efficient handling</li>
  </ul>
  
  <li><b>Label Encoding:</b></li>
  <ul>
    <li>Categorical language labels were encoded into numerical format, facilitating model training</li>
  </ul>
  
  <li><b>Deep Learning Models</b></li>
  <ul>
    <li>DNN, CNN, and RNN were implemented as part of the custom architecture</li>
    <li>DNNs excel at capturing complex relationships in high-dimensional data</li>
    <li>CNNs are adept at extracting spatial features, beneficial for speech patterns</li>
    <li>GRUs were employed to capture temporal dependencies inherent in spoken language</li>
  </ul>

  <li><b>Deep Learning Models</b></li>
   <ul>
    <li>Model performance was assessed on the testing set, evaluating metrics such as accuracy, precision, recall, and F1-score</li>
    <li>Comparative analysis was conducted to determine the efficacy of the combined DNN, CNN, and GRU architecture</li>
  </ul>

</ol>
