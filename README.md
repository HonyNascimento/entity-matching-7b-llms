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

- **Abt-Buy**: [Download direto](https://pages.cs.wisc.edu/~anhai/data/Structured/products/Abt-Buy.zip)
- **Walmart-Amazon**: [Download direto](https://pages.cs.wisc.edu/~anhai/data/Structured/products/Walmart-Amazon.zip)

Use o script `scripts/download_datasets.py` para baixar automaticamente.

---

## ⚙️ Requisitos

- Python 3.12+
- Ollama 0.1.22+
- 11 GB de VRAM (GTX 1080 Ti ou superior)

Instale os pacotes:

```bash
pip install -r requirements.txt
