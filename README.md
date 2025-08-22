# 📊 Base de Dados Fictícia - Corretora de Valores

Este repositório contém uma base de dados **fictícia** com 15.000 clientes de uma corretora de valores no Brasil.  
O objetivo é simular um dataset realista, com **inconsistências propositalmente adicionadas**, ideal para estudos de **limpeza, tratamento e análise de dados**.

---

## 📂 Estrutura do Arquivo

- **Arquivo:** `base_clientes_corretora.csv`  
- **Formato:** CSV separado por `;`  
- **Linhas:** 15.000  
- **Colunas principais:**
  - `ID_Cliente`: identificador único  
  - `Nome_Completo`  
  - `Idade`  
  - `Sexo` (M, F, outros valores ou nulos)  
  - `CPF` (fictício, formato válido)  
  - `Estado` (UF)  
  - `Cidade`  
  - `Região` (com erros como `sudets`, `noredeste`, etc.)  
  - `Tempo_de_Casa` (anos de relacionamento, incluindo valores quebrados)  
  - `Perfil_Investidor` (Conservador, Moderado, Arrojado, com variações incorretas)  
  - `Patrimonio_Total (R$)`  
  - `Distribuição_Carteira` (Renda Fixa, Ações, Fundos Imobiliários, Cripto, ETFs, Tesouro Direto – podendo não somar exatamente 100%)  
  - `Valor_Pago_Corretora (R$)`  
  - `Data_Cadastro`  
  - `Ultimo_Acesso_Plataforma` (com alguns erros de consistência)  
  - `Ativo` (Sim, Não, S, N, Atv, nulos)

---

## 🌍 Distribuição Geográfica
- **45%** dos clientes em **SP**  
- **15%** no **RJ**  
- **10%** em **MG**  
- **15%** no **Sul (PR, SC, RS)**  
- **15%** no restante do Brasil  

---

## 💰 Perfis de Investidor
- **Conservador** → patrimônio até R$ 200 mil, foco em Renda Fixa e Tesouro Direto  
- **Moderado** → patrimônio entre R$ 200 mil e R$ 1 milhão, diversificação entre Fundos e Ações  
- **Arrojado** → patrimônio acima de R$ 1 milhão, exposição a Ações, Cripto e ETFs  

---

## 🚀 Como Usar

### Google Colab
```python
import pandas as pd

url = "https://raw.githubusercontent.com/WalAmoedo/Base-de-dados-/main/base_clientes_corretora.csv"
df = pd.read_csv(url, sep=";")
df.head()


🎯 Objetivo

Esta base pode ser usada para:

Treinar técnicas de ETL (Extract, Transform, Load)

Exercícios de limpeza de dados e tratamento de inconsistências

Análises de perfil de cliente, receita da corretora e patrimônio

Estudos em SQL, Python, Power BI e ferramentas de Data Analytics

⚠️ Observação: Todos os dados são fictícios e foram gerados apenas para fins educacionais.
