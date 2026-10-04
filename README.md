[readme_md.md](https://github.com/user-attachments/files/33017975/readme_md.md)

# 📊 Sistema de Gestão e Dashboard de Vendas

Aplicação web interativa desenvolvida em Python para registro de transações comerciais, atualização de base de dados e visualização de indicadores de desempenho de vendas em tempo real.

---

## 🛠️ Tecnologias e Ferramentas

* **Linguagem:** [Python](https://www.python.org/)
* **Interface Web:** [Streamlit](https://streamlit.io/) — framework voltado para construção ágil de aplicações de dados e dashboards.
* **Processamento e Estruturação de Dados:** [Pandas](https://pandas.pydata.org/) — manipulação tabular, agregação e persistência em CSV.
* **Visualização Analítica:** [Plotly Express](https://plotly.com/python/) — geração de gráficos dinâmicos e interativos.

---

## 🧠 Competências e Conceitos Aplicados

Durante o desenvolvimento deste projeto, foram consolidados os seguintes conceitos técnicos e práticos:

### 1. Prototipagem e Desenvolvimento de Interfaces (Streamlit)
* **Organização de Layout:** Divisão lógica da aplicação entre controles laterais (`st.sidebar`) e painel principal de métricas e visualizações.
* **Componentes de Entrada Interativos:** Captura de parâmetros com tipagem consistente utilizando `st.date_input`, `st.selectbox` e `st.number_input`.
* **Tratamento de Eventos e Feedback Visual:** Acionamento de rotinas a partir de cliques (`st.button`) e emissão de mensagens de estado (`st.success`).

### 2. Manipulação e Persistência de Dados (Pandas)
* **Carga e Leitura de Arquivos:** Importação de bases de dados estruturadas a partir de arquivos `.csv` com `pd.read_csv`.
* **Mutação de DataFrames:** Inserção dinâmica de novos registros no DataFrame utilizando indexação por localização (`DataFrame.loc[]`).
* **Persistência em Disco:** Gravação consistente das alterações diretamente no arquivo físico via `to_csv(index=False)`.

### 3. Business Intelligence e Visualização (Plotly)
* **Cálculo de Indicadores (KPIs):** Agregação matemática dos valores totais de venda (`Series.sum()`) e exibição formatada com `st.metric`.
* **Análise Comparativa Multidimensional:** Construção de gráfico de barras com segmentação categórica por produto (`px.bar(..., color="produto")`) para avaliar faturamento individual por vendedor.
* **Análise de Composição Percentual:** Criação de gráfico de setores (`px.pie`) para mapear a participação de cada produto no faturamento total.

---

## 📁 Estrutura de Arquivos

```text
├── codigo.py          # Script principal contendo interface, lógica e gráficos
├── vendas.csv         # Base de dados estruturada das transações
├── requirements.txt   # Dependências do projeto
└── README.md          # Documentação do projeto
```

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
* Python 3.8 ou superior instalado.

### 1. Clonar ou Baixar o Repositório
```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```

### 2. Instalar as Dependências
```bash
pip install -r requirements.txt
```

### 3. Iniciar a Aplicação
```bash
streamlit run codigo.py
```

Acesse o endereço exibido no terminal (geralmente `http://localhost:8501`) no seu navegador.
