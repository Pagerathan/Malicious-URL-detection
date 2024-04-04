> # DETECTION OF MALICIOUS URL USING MACHINE LEARNING APPROACH 

***

 **Word-Level CNNs:**
   - Unique words identified in training corpus.
   - Words converted to matrix representation for CNN application.
   - Special token <UNK> used for rare words.
   - Unseen words in test URLs replaced with <UNK>.

 **Special Characters as Words:**
   - Proposal to include special characters as unique words.
   - Special characters offer valuable information for URL context.
   - Consideration of special characters improves detection accuracy.

 **Improved Word Embedding:**
   - Character-level embedding used to address memory constraints.
   - Word embedding obtained by combining original word and character embeddings.
   - Character-level word embedding captures subword information effectively.

**Model Configuration:**
   - Model overview: character-level and word-level branches.
   - Convolutional operations applied to both branches.
   - Fully connected layers with dropout regularization.
   - Optimized using Backpropagation.

 **Feature Extraction:**
   - Lexical features extracted from raw URLs.
   - BoW, URL component tokenization, position-sensitive bigrams, character trigrams.
   - Statistical properties like URL length, hostname length, and dot count considered.

 **Word-frequency Distribution:**
   - Analysis of word frequency distribution.
   - Over 90% of unique words in training corpus appear only once.
   - Ignoring rare words resolves memory issues and enables training on large datasets.

**Results:**
   - Comparison with baseline SVM models on AUC and TPR@FPR metrics.
   - Project outperforms baselines, capturing semantic and structural URL information effectively.
   - Project combines character-level and word-level information for improved performance.

**Visualization:**
   - Feature vector comparison between Project and baseline models.
   - Project effectively separates malicious and benign URLs.
   - Clustering analysis reveals patterns indicative of malicious or benign nature.

**Ablation Analysis:**
    - Component-wise performance evaluation of Project.
    - Special characters as words and character-level word embedding improve AUC scores.
    - Project integrates features for consistent performance improvement.

 **Related Work:**
    - Brief overview of feature representation and deep learning in malicious URL detection.
    - Project novel approach surpasses traditional bag-of-words methods.

**Conclusion:**
    - Project proposed as CNN-based model for malicious URL detection.
    - End-to-end approach eliminates need for manual feature engineering.
    - Advanced word embedding techniques address challenges of rare words and unseen features.
    - Project achieves superior performance through joint optimization of character and word-level information.- Developed a malware detection system to predict which feature will result in the file most likely being malicious or not.
- Implemented standardization of data to help in feature extraction using CNN and categorisation.
- Found the suitable algorithm for the given dataset ( data had some noise which may result in overfitting ) by implementing various methods KNN, Random Forest in classification.
- Used Random forest in learning algorithm as it resulted in the graph having maximum detection rate and lowest false positive rate.

  ***
