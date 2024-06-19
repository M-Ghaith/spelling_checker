# spelling_checker
Implements a spelling checker using a statistical language mode by leveraging frequency data from a lexicon and a pre-processed corpus.

## Requirements

The following files are required to run the notebook:

- `sentences_with_typos.txt`: A file with two tab-separated columns, the first containing a numerical ID and the second containing a sentence in English with potential spelling errors.
- `SUBTLEXus.txt`: A file with several tab-separated columns, containing data from the SUBTLEXus lexicon, a list of words derived from a part of the SUBTLEXus corpus containing movie subtitles with their frequency counts (and other pieces of information).
- `LM_trainingCorpus.json`: A file containing a pre-processed corpus in the form of a list of lists of strings, to be used to train a word-level statistical language model.

## Tasks

### Task 1

Complete the docstrings for the statistical language model implementation. The notebook provides a blueprint for the docstrings that need to be filled out.

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

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## Contact

For any questions or suggestions, please contact [your-email@example.com].


