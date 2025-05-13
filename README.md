# entity-matching-7b-llms
Reprodução do paper: Entity Matching with 7B LLMs

Este repositório contém a reprodução dos experimentos descritos no artigo:

> **Entity Matching with 7B LLMs: A Study on Prompting Strategies and Hardware Limitations**

## 🔍 Objetivo

Explorar o uso de modelos de linguagem de 7 bilhões de parâmetros quantizados para realizar *Entity Matching*, utilizando diferentes estratégias de prompting (zero-shot, few-shot, domain-specific).

---

## 📁 Estrutura do Projeto

- `data/`: Dados originais dos experimentos (Abt-Buy, Walmart-Amazon)
- `scripts/`: Scripts Python para baixar datasets, aplicar prompts e gerar métricas
- `models/`: Código para rodar os modelos via Ollama
- `prompts/`: Exemplos dos prompts utilizados (zero-shot, few-shot)
- `results/`: Métricas (F1, precisão, recall) e gráficos comparativos
- `notebooks/`: Análises e testes exploratórios

---

## 📦 Datasets

Os datasets utilizados foram:

- **Abt-Buy**:
[Link](https://paperswithcode.com/dataset/abt-buy)
[Download direto](https://dbs.uni-leipzig.de/files/datasets/Abt-Buy.zip)
- **Walmart-Amazon**:
[Link](https://www.kaggle.com/datasets/satriowp/amazonwalmart-dataset?resource=download&SSORegistrationToken=CfDJ8KT8tnOr7fFFm_byYmusL7h5Ty19or31iMUbEDc69D6JJj5V58Gr-d6lJ4HJkStuuZ8KpAqQ9GdoXf0FoxrVLXdroisIQzkqb7h8f-tke0w3X0fw8Kkim5FOpjR7wHrjPKlKPquGUQ27cGN1vR9NtC1uLmwvQ_ajiD6_eIlJkilQicMeK4bpcQxH9bdUEF1QrUDh1WdFniYvAAhL-BW53GkMXbeG7Uprj8uTxWybyalKY1oAL7q62gX1BosGDkmLqf_4Jm2hmtNM-KMwvja6wc8kBJ0eierSchIiiny0HYQWDp7NZvOdK7OtEgUefAXgAUlnkRm6cMoDT0_fWPA4HXM&DisplayName=Hony%20A%20Nascimento)

---

## ⚙️ Detalhes Hardware e Software Utilizados

- Python 3.13.3
- Ollama 0.6.0
- 11 GB de VRAM (GTX 1080 Ti ou superior)

Instale os pacotes:

```bash
pip install -r requirements.txt
