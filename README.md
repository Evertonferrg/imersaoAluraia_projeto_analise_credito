Sistema de Análise de Crédito
Visão Geral
Este sistema de análise de crédito é uma aplicação desenvolvida para avaliar o risco de crédito de empresas, utilizando o modelo de linguagem Gemini. O sistema coleta informações sobre a empresa, avalia o risco de crédito e gera um relatório detalhado.

Funcionalidades
Busca de Informações da Empresa: O sistema pode buscar informações públicas sobre a empresa usando o nome ou CNPJ, através do Google.

Entrada Manual de Dados: O usuário pode inserir as informações da empresa manualmente, caso a busca automática não seja suficiente.

Avaliação de Risco de Crédito: O sistema avalia o risco de crédito da empresa com base nas informações coletadas, atribuindo uma nota de risco de 1 a 5.

Geração de Relatório de Crédito: O sistema gera um relatório completo com a avaliação de risco, justificativa e informações detalhadas da empresa.

Geração de Gráfico de Risco: O sistema gera um gráfico de barras para visualizar a nota de risco da empresa.

Tecnologias Utilizadas
Como Usar
Configuração:

Configure a API Key do Google Gemini no Google Colab, armazenando-a na seção de dados do usuário com a chave GOOGLE_API_KEY.

Execução:

Execute o script principal (main).

O sistema irá solicitar a forma de entrada de dados (busca automática ou manual).

Siga as instruções para fornecer as informações da empresa.

O sistema irá gerar o relatório de crédito e o gráfico de risco.

Requisitos
Python 3.6 ou superior

Bibliotecas Python: os, google.colab, google.generativeai, IPython.display, google.adk, datetime, textwrap, warnings, pandas, altair

API Key do Google Gemini

Instalação
Clone este repositório:

git clone https://github.com/Evertonferrg/imersaoAluraia_projeto_analise_credito/blob/9f03eef900ba1f723a48f9cbb2412749de62ccf4/imersaoalura_sistema_analise_credito.ipynb

Instale as dependências:

pip install -r requirements.txt

Nota: Certifique-se de ter o pip instalado. Se estiver usando o Google Colab, as dependências já estão inclusas.

Configure a API Key do Google Gemini no Google Colab.

Exemplo de Uso
O usuário executa o script main.

O sistema pergunta se o usuário deseja buscar as informações da empresa automaticamente ou inseri-las manualmente.

O usuário escolhe a opção 1 (busca automática) e insere o CNPJ do Banco do Brasil (00.000.000/0001-91).

O sistema busca as informações da empresa e as exibe.



pautei.com
O sistema avalia o risco de crédito do Banco do Brasil e exibe a nota de risco e a justificativa.



www.sydle.com
O sistema gera um relatório de crédito completo e o exibe.



pt.venngage.com
O sistema gera um gráfico de barras representando a nota de risco e o exibe.




Estrutura do Código
* `main()`: Função principal que coordena a execução do sistema.
* `buscar_info_empresa(nome_ou_cnpj)`: Agente para buscar informações da empresa usando o Google.
* `coletar_informacoes_manuais()`: Função para coletar informações da empresa diretamente do usuário.
* `avaliar_risco_credito(informacoes)`: Agente para avaliar o risco de crédito da empresa.
* `gerar_relatorio_credito(nome_empresa, avaliacao_risco, justificativa_risco, informacoes)`: Função para gerar o relatório de crédito.
* `gerar_grafico_risco(avaliacao_risco)`: Função para gerar o gráfico de risco.
* `call_agent(agent, message_text)`: Função auxiliar para interagir com os agentes.
* `to_markdown(text)`: Função auxiliar para formatar o texto em Markdown



Nota
Este sistema foi desenvolvido para fins de estudo e demonstração. A avaliação de risco de crédito é simplificada e não deve ser utilizada para decisões financeiras reais.
