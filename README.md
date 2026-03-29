# 📊 Projeto de Ciência de Dados — Camadas Bronze e Prata

Este projeto tem como objetivo construir um pipeline de dados utilizando a arquitetura em camadas (**Bronze → Prata**), a partir de dados de incidentes de segurança cibernética, seus impactos financeiros e impactos no mercado.

---

# 📁 Estrutura do Projeto

```
data/
 ├── raw/        # Dados brutos (CSV - não versionados)
 ├── bronze/     # Dados estruturados em Parquet
 └── prata/      # Dados tratados e prontos para análise
pipeline.ipynb
```

---

# ⚠️ Sobre os Dados

Os arquivos CSV não estão incluídos neste repositório.

*Para executar o projeto, você deve adicionar manualmente os arquivos na pasta:*

```
data/raw/
```

Arquivos esperados:

* `incidents_master.csv`
* `financial_impact.csv`
* `market_impact.csv`

---

# 🧰 Pré-requisitos

Antes de começar, você precisa ter instalado:

* Python 3.10 ou superior
* pip (gerenciador de pacotes do Python)

---

# 🐍 Criando o Ambiente Virtual

No terminal, dentro da pasta do projeto:

```bash
python3 -m venv venv
```

---

# ▶️ Ativando o Ambiente Virtual

### 🐧 Linux / Ubuntu / Zorin OS

```bash
source venv/bin/activate
```

### 🪟 Windows

```bash
venv\Scripts\activate
```

---

# 📦 Instalando as Dependências

Com o ambiente ativado:

```bash
pip install -r requirements.txt
```

---

# 📝 Exemplo de requirements.txt

Caso ainda não tenha, crie um arquivo `requirements.txt` com:

```
pandas
numpy
matplotlib
seaborn
pyarrow
openpyxl

```

---

# 🚀 Executando o Projeto

1. Coloque os arquivos CSV em:

```
data/raw/
```

2. Execute os scripts ou notebooks para:

### 🥉 Gerar a camada Bronze

* Conversão de CSV → Parquet
* Padronização de colunas

### 🥈 Gerar a camada Prata

* Tratamento de dados
* Remoção de colunas irrelevantes
* Tratamento de valores nulos

---

# 🔄 Fluxo do Pipeline

```
RAW (CSV)
   ↓
BRONZE (Parquet estruturado)
   ↓
PRATA (dados tratados)
```

---

# 📌 Observações

* Os dados não são versionados no repositório (boas práticas de engenharia de dados)
* Apenas a estrutura de pastas é mantida
* O projeto pode ser facilmente reproduzido adicionando os dados na pasta `raw`

---
