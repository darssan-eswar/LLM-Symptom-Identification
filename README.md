## Text Extraction/Classification of User Posts

This repository contains a set of Jupyter notebooks designed to extract symptoms from mental health stories using poopular open-source large language models.

## Overview

The primary goal of this project is to utilize AI models to extract and categorize specific symptoms from user-generated text based on standardized mental health assessments, such as the GAD-7 (Generalized Anxiety Disorder-7) and PHQ-9 (Patient Health Questionnaire-9). The methods used here can be adapted for other forms of text analysis, symptom extraction, or commmon text extraction and evaluation tasks.

**Key Features**:
- **JSON Input and Output**: The notebooks handle JSON objects containing mental health stories, extracting specific sentences linked to various symptoms.
- **AI-Based Text Extraction**: Utilized the [GROQ API](https://groq.com) to process JSON objects containing mental health stories and extract symptoms based on the GAD-7 and PHQ-9 questionnaires. Each script contains an AI-generated case used for prompting.
- **Automation and Scalability**: The provided notebooks can be scaled to process large datasets, allowing for efficient extraction of symptom-related data.

## Files Included

- PHQ-9-llama-3.1-8b-groq.ipynb: [Google Colab Link](https://colab.research.google.com/drive/1f2zeP4hwc_AQYRDHVDni7rOxGtRpwnyp?usp=sharing)
- GAD-7-llama-3.1.ipynb: [Google Colab Link](https://colab.research.google.com/drive/1nSn8kvCU9AKuFufdQG7BulAp0-eUVmum?usp=sharing)
- PHQ-9-mixtral-groq.ipynb: [Google Colab Link](https://colab.research.google.com/drive/1JLGiDzc2nriev7B9W4ZkzWPyrIWVP-zL?usp=sharing)
- GAD-7-mixtral.ipynb: [Google Colab Link](https://colab.research.google.com/drive/12lnsjFcYXzPjOCg0XVTZrkN-vft4_ZaL?usp=sharing)
- **`README.md`**: This documentation file.

## How to Use

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/Symptom-Extraction.git
    cd Symptom-Extraction
    ```

2. **Run the Notebooks**:
    Open the notebooks in Jupyter Notebook or Google Colab and run the cells sequentially. Each notebook is designed to process a sample JSON file, generate outputs, and save the results to a new JSON file.

3. **Configuration**:
    - Replace placeholder API keys with your own API secret keys in the code sections.
    - Modify input and output paths as necessary to suit your data structure.

## JSON Input Format

The input files are expected to be in JSON format, containing objects with text fields and annotations. Each object should include:
- `post_title`: Title of the mental health story.
- `post_text`: Main content of the story.
- `annotations`: Empty arrays for symptoms to be filled based on the text content.

## Output

The output JSON files contain the original story with extracted sentences for each symptom, preserving the structure of the input data while adding detailed symptom annotations.

## Disclaimer

This project is intended for research and demonstration purposes. The outputs should not be used as a substitute for professional mental health evaluation or diagnosis. Ensure that sensitive data is handled securely, and comply with ethical standards when working with mental health-related content.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

