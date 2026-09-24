### Sentiment Classification with a Bidirectional LSTM
**Tools: Python, TensorFlow/Keras, GloVe embeddings, scikit-learn, pandas** | M.S. Data Analytics Project (D213 - Advanced Data Analytics)

I trained a neural network to classify customer reviews as positive or negative, combining labeled review data from Amazon, Yelp, and IMDb to test whether sentiment patterns generalize across domains.
 
- Profiled raw text before modeling, identifying 2,748 emojis and several non-ASCII characters, and normalized the text with regular expressions
- Set a maximum sequence length statistically (mean plus two standard deviations) rather than padding to the longest review, reducing unnecessary padding
- Tested a heuristic 9-dimension embedding, found it underperformed, and switched to frozen 100-dimension pretrained GloVe embeddings
- Built a bidirectional LSTM with dropout and early stopping, reaching about 80% test accuracy with closely aligned training and validation performance

[Documentation](https://github.com/hrbergman/review-sentiment-lstm/blob/main/review-sentiment-lstm/sentiment-analysis-lstm-documentation.pdf)

