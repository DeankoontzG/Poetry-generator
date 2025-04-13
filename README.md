# Poetry-generator
The goal of this project is to implement a text generator for poetry, using neural networks.
Its objective is to train an AI model on the poetry of Charles Baudelaire, Arthur Rimbaud, and the French rapper Lorenzo, allowing it to generate text in their style.

Different versions of the model were implemented:

## Models Used

### 1. Long short-term memory (LSTM)
By using an LSTM-type neural network, the goal was to create an accurate model with a strong focus on long-term memory in order to generate meaningful sentences.
- Tokenized by words, focusing on generating grammatically correct text, but at the expense of creativity.
- The model was trained for only 20 epochs due to its high resource consumption and the long training times required by LSTM. Further exploration with more frugal models might be necessary for continued progress.
- Results: While the model produced coherent vocabulary within poems, it struggled with syntax and the use of linking words. Possible causes: insufficient training data and the tendency of Lorenzo's texts to deviate from conventional syntax. Without Lorenzo's texts, the results improved, but the model still wasn't quite there.

**Improvement process :**
- Splitting data in training & testing sets, computing & comparing both during each epoch to verify if there was Overfitting => No meanningfull difference observed during 20 epochs, no overfitting
- 

### 2. Gate Recurrent Unit (GRU)
The goal was this time to use a simpler model, allowing it to be trained for more Epochs. It reuses basically the same code that the LSTM model for the most part.
- Tokenized on words too
- Training increased : epoch = 50
- Results : 
