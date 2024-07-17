FastText Python Module
This Python module provides an interface to the FastText library for efficient learning of word representations and text classification.

**Installation**:

To use this module, ensure you have FastText installed. You can install FastText and its Python bindings using pip:
pip install fasttext
****

**Usage**

Loading a Model

  _Python Code:_

    from fasttext_module import load_model
    model = load_model("path/to/model.bin")


Using the Model
Word Vectors
  
  _Python Code_:
  
    vector = model.get_word_vector("example_word")

Sentence Vectors

  _Python Code_:

    vector = model.get_sentence_vector("This is an example sentence.")

Predictions

  _Python Code_:

    labels, probabilities = model.predict("input text")

Training

Supervised Training

  _Python Code_:

    from fasttext_module import train_supervised
    model = train_supervised(input="train.txt")

Unsupervised Training

  _Python Code_:

    from fasttext_module import train_unsupervised
    model = train_unsupervised(input="text.txt")
  
****

**API Reference**

Class: _FastText

  Methods:
  
    'get_word_vector(word)'
    'get_sentence_vector(text)'
    'predict(text)'
    'train_supervised(*kargs, **kwargs)'
    'train_unsupervised(*kargs, **kwargs)'
    
Class: _Meter
      
  Methods:
  
    'score_vs_true(label)'
    'precision_recall_curve(label)'
    'precision_at_recall(recall, label)'
    'recall_at_precision(precision, label)'
****

**License**
This project is licensed under the MIT License. See the LICENSE file for details.
****

