# 🎲 Dashboard de Análise na Área de Dados

Um painel interativo construído com Python e Streamlit para explorar, visualizar e analisar tendências salariais globais de profissionais da área de dados. 

Este projeto processa dados reais para extrair insights valiosos sobre como fatores como experiência, tipo de contrato e localização geográfica impactam a remuneração no setor de tecnologia.

## 🚀 Funcionalidades

* **Filtros Dinâmicos:** Refine a análise na barra lateral selecionando Ano, Nível de Senioridade, Tipo de Contrato e Tamanho da Empresa.
* **Métricas Principais (KPIs):** Visualização rápida do salário médio, salário máximo, volume de registros e cargo mais frequente baseado nos filtros aplicados.
* **Análises Visuais:**
    * 🏆 **Top 10 Cargos:** Gráfico de barras horizontais detalhando as funções com as maiores médias salariais.
    * 📊 **Distribuição Salarial:** Histograma demonstrando a concentração e dispersão dos salários anuais em USD.
    * 🍩 **Modelos de Trabalho:** Gráfico de rosca exibindo a proporção entre trabalho remoto, presencial e híbrido.
    * 🗺️ **Mapa Global (Data Science):** Mapa coroplético ilustrando o salário médio de Cientistas de Dados distribuído por país.
* **Tabela de Dados:** Acesso direto aos dados brutos e filtrados para consultas específicas.

## 🛠️ Tecnologias Utilizadas

[cite_start]As principais bibliotecas utilizadas neste projeto são[cite: 1]:

* [cite_start]**Pandas (>=2.2.3):** Para manipulação e análise dos dados. [cite: 1]
* [cite_start]**Streamlit (==1.44.1):** Para a construção da interface web interativa do dashboard. [cite: 1]
* [cite_start]**Plotly (==5.24.1):** Para a renderização dos gráficos dinâmicos e do mapa. [cite: 1]

## ⚙️ Como Executar o Projeto Localmente

Siga os passos abaixo para rodar o dashboard na sua própria máquina:

**1. Clone o repositório:**
`bash
git clone https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git
cd NOME_DO_REPOSITORIO
`

**2. Crie um ambiente virtual (Recomendado):**
`bash
python -m venv venv
# No Windows:
venv\Scripts\activate
# No Linux/Mac:
source venv/bin/activate
`

**3. Instale as dependências:**
`bash
pip install -r requirements.txt
`

**4. Execute a aplicação:**
`bash
streamlit run app.py
`

O dashboard abrirá automaticamente no seu navegador padrão, geralmente no endereço `http://localhost:8501`.

## 📁 Fonte de Dados

Os dados utilizados neste painel são carregados remotamente via arquivo CSV hospedado no GitHub, garantindo que o dashboard reflita a versão mais recente e consolidada da base (`dados-imersao-final.csv`).

## 🔮 Melhorias Futuras (Roadmap)

Este projeto está em evolução. Algumas das melhorias planejadas incluem:

* **Integração com Banco de Dados:** Substituir a leitura direta do CSV estático por uma conexão com um banco de dados relacional (ex: PostgreSQL) ou NoSQL para lidar com volumes maiores de dados.
* **Cobertura de Testes de Software:** Implementar testes unitários (utilizando `pytest`, por exemplo) para garantir o funcionamento correto das funções de filtragem e processamento do Pandas.
* **Deploy em Nuvem (Cloud Computing):** Hospedar a aplicação em serviços de nuvem para torná-la acessível publicamente com maior escalabilidade.
* **Pipeline de CI/CD:** Configurar fluxos de trabalho (ex: GitHub Actions) para automatizar a execução de testes e o deploy a cada novo commit.
