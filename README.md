# Análise de Cancelamento de Clientes

Projeto desenvolvido em **Python** com o objetivo de analisar dados de cancelamento de clientes para identificar os principais motivos de cancelamento e propor ações eficientes para reduzir esse número. Esta ferramenta é ideal para empresas que precisam entender o comportamento de seus clientes e melhorar a retenção.

---

## Objetivo
O projeto realiza uma análise completa de uma base de dados de clientes para identificar padrões e causas de cancelamento, como:
* Tipo de contrato (mensal, trimestral, anual)
* Número de ligações ao call center
* Atrasos no pagamento
* Frequência de uso do serviço
* Tempo como cliente
* Outros fatores demográficos e comportamentais

---

## Tecnologias Utilizadas
* **Python**
* **Pandas** (Manipulação e análise de dados)
* **Plotly** (Visualização de dados interativa)
* **Jupyter Notebook** (Ambiente de desenvolvimento e análise)

---

## Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/gabgrisolia/automacao-cadastro-produtos.git](https://github.com/gabgrisolia/automacao-cadastro-produtos.git)
    cd automacao-cadastro-produtos
    ```

2.  **Instale as bibliotecas necessárias:**
    Você precisará do Pandas, Plotly e Jupyter. Instale todos de uma vez com o comando:
    ```bash
    pip install pandas plotly openpyxl nbformat ipykernel
    ```

3.  **Prepare a base de dados:**
    Certifique-se de que o arquivo de dados `cancelamentos.csv` esteja na mesma pasta do notebook.

4.  **Execute o notebook:**
    ```bash
    jupyter notebook inicial.ipynb
    ```
    Ou abra o arquivo `inicial.ipynb` em seu ambiente Jupyter preferido e execute as células sequencialmente.

---

## Funcionamento do Script

1.  **Importação:** O script importa a base de dados usando **Pandas** e remove a coluna `CustomerID`.
2.  **Visualização:** Exibe informações sobre a estrutura da base de dados e identifica possíveis problemas.
3.  **Tratamento:** Remove valores nulos e corrige problemas na base de dados.
4.  **Análise Inicial:** Calcula a quantidade e porcentagem de clientes que cancelaram.
5.  **Análise Detalhada:** Cria gráficos interativos com **Plotly** para cada coluna, comparando clientes que cancelaram com os que permaneceram.
6.  **Filtragem e Insights:** Identifica padrões críticos e aplica filtros para validar hipóteses sobre as causas de cancelamento.

---

## Principais Descobertas

Com base na análise dos dados, foram identificados três fatores críticos que levam ao cancelamento:

* **Contrato Mensal:** Todos os clientes com contrato mensal cancelaram o serviço.
  * **Ação:** Oferecer desconto para contrato anual ou trimestral.

* **Ligações ao Call Center:** Clientes com mais de 4 ligações ao call center cancelaram.
  * **Ação:** Se o cliente ligar 3 vezes para o call center, criar alerta vermelho para atendimento prioritário.

* **Atraso no Pagamento:** Clientes com atraso acima de 20 dias cancelam.
  * **Ação:** Se o cliente atrasar 15 dias no pagamento, criar alerta vermelho para ação preventiva.

---

## Autor
Gabriela Grisolia | Projeto educacional (Hashtag Treinamentos)
* GitHub: [gabgrisolia](https://github.com/gabgrisolia)
