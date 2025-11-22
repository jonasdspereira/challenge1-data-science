# AluraStoreBrasil — Análise das Lojas

Este repositório contém o notebook `AluraStoreBrasil.ipynb`, que realiza uma análise exploratória de vendas de quatro lojas (faturamento, categorias, produtos mais vendidos, avaliações e frete). O objetivo é recomendar a melhor loja para o Senhor João vender com base nas métricas analisadas.

**Estrutura do repositório**

- `AluraStoreBrasil.ipynb` — notebook principal com carregamento dos dados, visualizações e relatório final.
- `base-de-dados-challenge-1/` — pasta com os arquivos CSV das lojas:
  - `loja_1.csv`
  - `loja_2.csv`
  - `loja_3.csv`
  - `loja_4.csv`
- `scripts/compute_metrics.py` — (opcional) script auxiliar criado que calcula métricas e imprime um relatório em Markdown.

**Objetivo da análise**

- Comparar o faturamento total entre lojas.
- Identificar categorias de produto com maior/menor faturamento.
- Avaliar a média das avaliações de clientes por loja.
- Listar produtos mais e menos vendidos (top/low sellers).
- Calcular o frete médio por loja.
- Gerar visualizações (barras, histogramas, boxplots, pizzas) e um relatório final com recomendação de venda.

Recomendações e critério padrão utilizado no notebook:

- O critério principal usado automaticamente para recomendação é o **faturamento total** (escolhe a loja com maior faturamento).
- Avaliações médias e frete médio são usados como critérios de desempate ou de ajuste (por exemplo, frete alto reduz margem e pode ser um sinal para negociação antes da venda).
- Você pode alterar a regra diretamente no notebook na célula do relatório caso queira priorizar avaliações ou frete.

Requisitos (instalação)

Os comandos a seguir funcionam no `cmd.exe` do Windows. Recomendamos criar/usar um ambiente virtual.

1. (Opcional) criar e ativar um venv:

```cmd
python -m venv .venv
.venv\Scripts\activate
```

2. Instalar dependências principais:

```cmd
pip install pandas matplotlib seaborn ipython
```

Execução do notebook

1. Abra `AluraStoreBrasil.ipynb` no Jupyter Notebook, JupyterLab ou VS Code (com suporte a notebooks).
2. Garanta que a pasta `base-de-dados-challenge-1/` esteja no mesmo diretório do notebook (já incluída no repositório). Caso os CSVs estejam em outro local, atualize os caminhos nas primeiras células.
3. Execute as células na ordem: carregamento dos dados → cálculos → visualizações → célula final do relatório.

