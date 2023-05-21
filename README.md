# PDF Papers Summarizer with ChatGPT
#### Author: Munir Jojo-Verge



This Python project is designed to summarize PDF documents using OpenAI's GPT-3 AI model. It reads PDF files from a given directory, counts the number of tokens in the text to manage usage of GPT-3, and uses GPT-3 to summarize the document. The summaries are then saved into Word (.docx) documents in a specified directory.

__It's mainly aimed to summarize papers for further analysis and code development. The summaries will include the key findings, methodology, experimental results, statistical analysis, and any limitations. The summary is formatted with bullet points for easy reference.__

## Features

- PDF text extraction using `pdfplumber`.
- Token counting using `tiktoken`.
- GPT-3 based text summarization using `openai`.
- Progress tracking with `tqdm`.
- Configuration handling with `hydra` and `omegaconf`.
- Document creation with `docx`.

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/munirjojoverge/pdf_summarize_chatGPT.git
    ```

2. Change into the directory:

    ```sh
    cd pdf_summarize_chatGPT
    ```

3. Create a simple conda/mamba enviroment and install the required packages:

    ```sh
    mamba env create -f environment.yaml
    mamba activate summarize
    ```

## Configuration

This project uses `hydra` for configuration. The config file is located at `config/config.yaml`. You can specify the openAI API key, the engine, and various other settings related to the GPT-3 model in this config file.

You also need to specify the path to the directory containing the PDF files to summarize, and the output directory where the summarized documents will be saved.

## Usage

After configuring the settings, you can run the project with the following command:

```sh
python pdf_summarize.py
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Disclaimer

This software is not guaranteed to be perfect and comes with no warranty. You should check the summarized documents for accuracy and completeness.

## Contact

Please raise an issue in this GitHub repository if you have any issues, questions, or feedback.
