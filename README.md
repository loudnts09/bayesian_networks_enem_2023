
# ENEM Bayesian Network — Execução rápida

Conteúdo: `RedesBayesianas_Dados_ENEM_2023.ipynb`, `requirements.txt`, e dados em `data/microdados_enem_2023/DADOS/` (`MICRODADOS_ENEM_2023.csv`, `ITENS_PROVA_2023.csv`).

Execução (Google Colab) — passos mínimos:
1. Abra `RedesBayesianas_Dados_ENEM_2023.ipynb` no Colab (upload ou via GitHub).
2. Instale dependências numa célula:

```python
!pip install --upgrade pip
!pip install pandas numpy matplotlib seaborn networkx pgmpy==0.1.25 pyvis pyarrow fastparquet plotly
```

3. Carregue os dados: faça upload dos CSVs ou monte o Google Drive e ajuste `DATA_DIR`:

```python
from google.colab import drive
drive.mount('/content/drive')
DATA_DIR = '/content/drive/MyDrive/path/to/data/microdados_enem_2023/DADOS'
```

4. Atualize `DATA_DIR` nas primeiras células do notebook e execute as células.

Execução local (opcional):

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
# depois: jupyter lab
```

Dados: coloque os CSVs originais do INEP em `data/microdados_enem_2023/DADOS/`.