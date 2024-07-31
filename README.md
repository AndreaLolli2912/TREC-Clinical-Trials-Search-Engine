# Clinical Trials Search Engine

This project was completed as a final examination for the course Information Retrieval and Recommender Systems, in collaboration with my colleagues [Kristian Perriù](https://github.com/kristianperriu) and [Chibuzor J. Amadi](https://github.com/chibuzoramadi). The goal is to create an intuitive platform that allows researchers and healthcare professionals to efficiently search and access information related to clinical trials based on textual descriptions of patients.

## Project Overview

### Task Description
We developed a search engine for clinical trials using PyTerrier, providing an easy-to-use platform for researchers and healthcare professionals to efficiently search and access information related to clinical trials, including trial descriptions, eligibility criteria, outcomes, and relevant publications.

### Method Outline

#### Dataset
The dataset comprises multiple columns with various details about specific clinical trials. The exact columns used were determined based on experimental results during the development phase.

#### Data Preprocessing
- **Text Preprocessing**: We applied techniques such as lowercasing, removing irrelevant special characters, punctuation, numbers, and stop-words.
- **Indexing**: We created two indexes – one for the main columns and another for exclusion criteria. This dual-index approach helped filter out irrelevant documents effectively.

#### Query Representation & Content Analysis
- **Query Representation**: We defined user queries using a combination of keywords and natural language to ensure comprehensive search results.
- **Content Analysis**: We incorporated contextual information such as medical history and current conditions into the search process.
- **LLM Implementation**: We implemented an LLM for content selection and entity recognition to enhance search accuracy.

#### Preprocessing & LLM Adoption
- We used an LLM for content selection and entity recognition on queries.
- We applied text preprocessing techniques while ensuring medical terms retained their meaning.

#### Query Form & Ranking
- **Single and Multiple Queries**: We developed a process for handling both single and multiple queries.
- **Ranking Techniques**: We experimented with ranking techniques including TF-IDF, BM25, and Cosine similarity.
- **Weighting Techniques**: We applied weighting techniques to guide the retrieval process to relevant documents.

### Resource References
- [Clinical Trials Database](https://clinicaltrials.gov/): A comprehensive database of clinical studies.
- [Research Paper on Medical IR](https://arxiv.org/pdf/2306.02077.pdf): Discusses advanced topics in medical information retrieval.
- [PyTerrier Documentation](https://pyterrier.readthedocs.io/en/latest/experiments.html): Guides for conducting experiments using PyTerrier.

This project provides a robust and user-friendly search engine for clinical trials, leveraging advanced information retrieval techniques and natural language processing to meet the needs of healthcare professionals and researchers.
