# CPI Data - Bureau of Labor Statistics (BLS)

Este repositório contém um **notebook em Python** para coletar dados do **Consumer Price Index (CPI)** diretamente da **API pública do Bureau of Labor Statistics (BLS)**.

## ▶️ Como usar no Google Colab
1. Abra o notebook [`cpi_data.ipynb`](./cpi_data.ipynb).
2. Clique em **"Open in Colab"** (ou abra no seu próprio Google Colab).
3. Execute as células para coletar e analisar os dados.

## 📊 Funcionalidades
- Consulta séries do CPI via API do BLS.
- Permite definir intervalo de anos e IDs das séries desejadas.
- Retorna os dados em formato `pandas DataFrame`.
- Organiza os dados em formato tabular (ano, mês, série, valor).
- Pivotagem para comparação entre diferentes séries.

## 📤 Exportar resultados
Caso queira salvar os dados em CSV:
```python
df_pivot.to_csv("cpi_data.csv", index=False)
