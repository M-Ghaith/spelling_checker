# spelling_checker
Implements a spelling checker using a statistical language mode by leveraging frequency data from a lexicon and a pre-processed corpus.

## Requirements

The following files are required to run the notebook:

- `sentences_with_typos.txt`: A file with two tab-separated columns, the first containing a numerical ID and the second containing a sentence in English with potential spelling errors.
- `SUBTLEXus.txt`: A file with several tab-separated columns, containing data from the SUBTLEXus lexicon, a list of words derived from a part of the SUBTLEXus corpus containing movie subtitles with their frequency counts (and other pieces of information).
- `LM_trainingCorpus.json`: A file containing a pre-processed corpus in the form of a list of lists of strings, to be used to train a word-level statistical language model.

## How to Use

1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Ensure you have the required files in the directory:
    - `sentences_with_typos.txt`
    - `SUBTLEXus.txt`
    - `LM_trainingCorpus.json`

3. Open the Jupyter Notebook:
    ```bash
    jupyter notebook spelling_checker.ipynb
    ```

4. Follow the instructions in the notebook to run the spelling checker and complete the tasks.

## Approaches Used
The spelling checker notebook employs the following approaches to correct spelling errors:

### Statistical Language Model:
Training: A statistical language model is trained using a pre-processed corpus (LM_trainingCorpus.json). This model learns the probability distribution of sequences of words, enabling it to predict the likelihood of a given sequence.
Error Correction: The language model is used to evaluate and rank candidate corrections for misspelled words based on their likelihood within the context of a sentence. This helps in selecting the most probable
correction for a given typo.

### Lexicon-Based Frequency Analysis:

Lexicon Data: The SUBTLEXus.txt file provides frequency counts of words derived from movie subtitles. This data is used to prioritize corrections based on the frequency of word usage in the English language.
Candidate Generation: Potential corrections for misspelled words are generated using the lexicon data. The more frequently a word appears in the lexicon, the higher its priority as a candidate correction.

### Contextual Analysis:

Sentence Context: The code considers the entire sentence context when determining the best correction for a misspelled word. By analyzing the surrounding words and their relationships, the model ensures that the corrected sentence maintains grammatical and semantic coherence.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## Contact

For any questions or suggestions, please contact [your-email@example.com].


