# RAG QA Pipeline

The project's aim is to create a Retrieval Augmented Generation-based Python application that can answer questions from documents provided as input data.

## Used Data

The data has been sourced from publicly accessible PDF files and websites of PwC Hungary. During the data acquisition process, no automated scraping tools were used. The data is intended solely for demonstration purposes.

## PDF File Sources

1. [Youth Employment Index 2024](https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/youth-employment-index-2024.pdf)  
2. [Invest in Hungary 2023](https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/investinhungary2023.pdf)  
3. [PwC 2024 Global Digital Trust Insights](https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/pwc-2024-global-digital-trust-insights.pdf)  
4. [PwC GEMO 2023](https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/pwc_gemo_2023.pdf)  
5. [PwC Global Top 100 Companies 2023](https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/pwc-global-top-100-companies-2023.pdf)  
6. [PwC Global Crisis Resilience Survey 2023](https://www.pwc.com/hu/hu/kiadvanyok/assets/pdf/pwc-global-crisis-resilience-survey-2023.pdf)

## HTML File Sources

1. [EVP 2024](https://www.pwc.com/hu/en/pressroom/2024/evp_2024.html)  
2. [Global Disclosure Obligations](https://www.pwc.com/hu/en/pressroom/2024/globe_bejelentesi_kotelezettseg.html)  
3. [Transfer Pricing Records Inspection](https://www.pwc.com/hu/en/pressroom/2024/transzferar_nyilvantartasok_ellenorzese.html)  
4. [GKID Purchases](https://www.pwc.com/hu/en/pressroom/2024/gkid_vasarlas.html)  
5. [New CEO Announcement](https://www.pwc.com/hu/en/pressroom/2024/uj_vezerigazgato.html)  
6. [10 New Directors Announcement](https://www.pwc.com/hu/en/pressroom/2024/10_uj_igazgato.html)

## Project Structure

- **Backend:** Hosts the Python backend part of the production application (not yet implemented).  
- **Frontend:** Hosts the frontend part of the production application (not yet implemented).  
- **Experiments:** Contains all experiments conducted by AI engineers to explore and evaluate new concepts and technologies before integrating them into the production code. This structure offers a separate sandbox, allowing AI engineers to work in parallel with traditional software developers.

## Current Progress

Currently, only the experiments are completed, and the solution is in an early Proof-of-Concept (POC) state.

## Frameworks and Technologies Used

- **Llama Index:** For implementing the RAG architecture of the AI application.  
- **ChromaDB:** Used as the vector database for the project.  
- **Ollama:** Simplifies LLM inference and enhances reproducibility.

## AI Models Used

- **Llama 3.2 3B**  
- **Nomic Embed Text**

## Project Setup

### LLM Setup

The project currently relies on Ollama to host the required LLMs.

1. Download the appropriate Ollama installer for your OS [here](https://ollama.ai).  
2. Install Ollama using the downloaded installer.  
3. After successful installation, open the Start menu, search for "Ollama," and launch it.  
4. Once Ollama is running in the background, open a command prompt and execute the following commands to install and run the required AI models:
   ```bash
   ollama run llama3.2
   ollama pull nomic-embed-text
