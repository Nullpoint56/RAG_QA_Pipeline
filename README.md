# RAG QA pipeline
The project's aim is to make a Retrieval Augmented Generation based Python application, that can answer questions from 
documents provided as input data to the application.

## Used data
Data has been sourced from publicly accessible PDF files and websites of PWC hungary. During the acquiring of the data, no automated scraping tools was used. The data is only used for demonstration purposes. 
- PDF file sources
  - https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/youth-employment-index-2024.pdf
  - https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/investinhungary2023.pdf
  - https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/pwc-2024-global-digital-trust-insights.pdf
  - https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/pwc_gemo_2023.pdf
  - https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/pwc-global-top-100-companies-2023.pdf
  - https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/pwc-global-crisis-resilience-survey-2023.pdf
- HTML file sources
  - https://www.pwc.com/hu/en/pressroom/2024/evp_2024.html
  - https://www.pwc.com/hu/en/pressroom/2024/globe_bejelentesi_kotelezettseg.html
  - https://www.pwc.com/hu/en/pressroom/2024/transzferar_nyilvantartasok_ellenorzese.html
  - https://www.pwc.com/hu/en/pressroom/2024/gkid_vasarlas.html
  - https://www.pwc.com/hu/en/pressroom/2024/uj_vezerigazgato.html
  - https://www.pwc.com/hu/en/pressroom/2024/10_uj_igazgato.html

## Project structure
- Backend: Hosts the python backend part of the production application. (not implemented)
- Frontend: Hosts the frontend part of the production application. (not implemented)
- Experiments: Contains all the experiments conducted by AI engineers to explore and evaluate new concepts and 
technologies before integrating them into the production code, offering a separated sandbox and allowing AI 
engineers to work in parallel with traditional software developers.

## Current progress
Currently, only the experiments are done and the solution is in early POC state.

## Frameworks and technologies used
- [Llama Index](https://www.llamaindex.ai/): For the implementation of the RAG architecture AI application
- [ChromaDB](https://www.trychroma.com/): As the vector database for the project
- [Ollama](https://ollama.com/): For easy LLM inference and to enhance reproducibility

## AI models used
- [Llama 3.2 3B](https://huggingface.co/meta-llama/Llama-3.2-3B)
- [Nomic Embed Text](https://huggingface.co/nomic-ai/nomic-embed-text-v1.5)

## Project setup
### LLM setup
The project currently relies on Ollama to host the used LLMs.
- [Download](https://ollama.com/download) the appropriate Ollama for your OS here
- Install Ollama using the downloaded installer
- After successful installation, go to the start menu and search for ollama, then start it.
- Once ollama is running in the background, open a command prompt and paste in the following commands to install and run the required AI models:
  - ```ollama run llama3.2```
  - ```ollama pull nomic-embed-text```
- Done, head over to [RAG_QA_pipeline.ipynb](experiments/notebooks/RAG_QA_pipeline.ipynb)
