<h1>Binary Disaster Tweet Classification Using NLP and Deep Learning</h1>

<p>This porject Also need Glove Embedding Files to run</p>

<p>This project implements a deep learning model to classify tweets as either related to a disaster or not. Using advanced NLP techniques, the model leverages architectures such as <strong>Bidirectional LSTM (Bi-LSTM)</strong> and <strong>Bidirectional GRU (Bi-GRU)</strong> to achieve reliable classification. The goal is to create a robust classifier that can distinguish disaster-related tweets, aiding in emergency response scenarios.</p>

<h2>Dataset</h2>
<p>The dataset, sourced from a Kaggle challenge, contains tweets with binary labels indicating whether each tweet is related to a disaster or not.</p>

<h3>Dataset Format</h3>
<p>The dataset is in CSV format with two main columns:</p>
<ul>
    <li><code>text</code>: The content of the tweet.</li>
    <li><code>target</code>: The binary label where <code>1</code> indicates a disaster-related tweet, and <code>0</code> denotes non-disaster content.</li>
</ul>

<h2>Preprocessing</h2>
<p>Text data is tokenized and standardized using padding to ensure consistent sequence length for model input.</p>

<h2>Model Architecture</h2>
<p>The model architecture includes multiple layers:</p>
<ul>
    <li><strong>Embedding Layer</strong>: Converts words into vectors, enhancing input representation.</li>
    <li><strong>Bidirectional LSTM and GRU Layers</strong>: Capture dependencies in the text from both directions for a nuanced understanding.</li>
    <li><strong>Dropout and Batch Normalization</strong>: Prevent overfitting and enhance generalization.</li>
    <li><strong>Fully Connected Layers</strong>: To consolidate learned features for final classification.</li>
</ul>

<h2>Results</h2>

<h3>Model Performance</h3>
<ul>
    <li><strong>Bi-LSTM</strong>:
        <ul>
            <li>Precision: 0.825</li>
            <li>Recall: 0.732</li>
            <li>F1 Score: 0.775</li>
        </ul>
    </li>
    <li><strong>Bi-GRU</strong>:
        <ul>
            <li>Precision: 0.832</li>
            <li>Recall: 0.784</li>
            <li>F1 Score: 0.807</li>
        </ul>
    </li>
</ul>

<h2>Evaluation Metrics</h2>
<p>A confusion matrix and classification report offer insights into the model's <strong>precision</strong>, <strong>recall</strong>, and <strong>F1-score</strong>, providing a detailed breakdown of performance across true positives, false positives, and other prediction metrics.</p>

<h2>Future Improvements</h2>
<p>Potential future improvements include:</p>
<ul>
    <li>Experimenting with transformer-based architectures such as <strong>BERT</strong> for improved accuracy.</li>
    <li>Utilizing data augmentation techniques to expand and diversify the training data.</li>
    <li>Further tuning hyperparameters to enhance model performance.</li>
</ul>
