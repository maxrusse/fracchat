

# AI Chatbots for Identifying AO Codes from Radiology Reports

This project leverages AI chatbots to classify radiology reports using the Arbeitsgemeinschaft Osteosynthesefragen (AO) Fracture and Dislocation Classification Compendium. We compare the performance of generic chatbots, context-aware chatbots, and human readers.

## Abstract
Radiologists adeptly describe fracture morphology. However, translating these into the AO classification is challenging. This project evaluates generic chatbots and context-aware chatbots informed by AO's vector-index. Chatbots identify AO codes faster than humans but have varied accuracy. Context-specific knowledge improves chatbot performance, suggesting that refined context is crucial for maximizing ChatGPT's potential.

## Using the Jupyter Notebook

1. Download the notebook file `Demo of AO Chatbots.ipynb`.
2. Upload the notebook to Google Colab, JupyterLab, or your preferred Jupyter notebook environment.
3. Set your OpenAI API key and the folder path containing the AO guidelines in the corresponding cells.
4. Execute the cells in the notebook to initialize the index, launch the interface, and interact with the AI chatbots.

## How It Works

The script utilizes various AI models to generate AO codes from radiology reports:
- **FracChat (using GPT4)**: Interrogates an index created from AO guidelines and retrieves the response using GPT-4.
- **FracChat (using GPT 3.5-Turbo)**: Uses GPT-3.5-Turbo to query the AO guidelines index.
- **GPT-3.5-Turbo**: Generates a response based on the GPT-3.5-Turbo model without context.
- **GPT-4**: Provides a response using the standalone GPT-4 model.

All model responses are aggregated and showcased in the interface.

## Setup using the Python Script

1. Acquire an OpenAI API key from [OpenAI](https://platform.openai.com/account/api-keys) and set the `OPENAI_API_KEY` environment variable in the script:
```python
os.environ["OPENAI_API_KEY"] = 'sk-ENTER_YOUR_API_CODE'
```
2. Specify the directory containing the AO guidelines in PDF format:
```python
FOLDER_PATH = "AO"
```
3. Execute the script to initiate the index and unveil the interface.

> Remember to provide a link to the full publication once it's available so interested parties can delve deeper into your research.
