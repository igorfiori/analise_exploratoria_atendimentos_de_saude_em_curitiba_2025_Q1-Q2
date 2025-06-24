# Análise Exploratória de Dados: Atendimentos de Saúde em Curitiba (2025 Q1/Q2)

## Sobre o Projeto

Este repositório contém uma Análise Exploratória de Dados (EDA) detalhada de aproximadamente **1 milhão de registros de atendimentos médicos** da rede de saúde pública de Curitiba, Paraná, referentes ao primeiro semestre de 2025.

O objetivo deste projeto foi ir além de uma análise superficial, realizando uma limpeza de dados rigorosa, uma engenharia de atributos inteligente e uma investigação visual profunda para extrair insights estratégicos sobre o funcionamento do sistema de saúde. A análise explora o perfil demográfico e clínico dos pacientes, a dinâmica geográfica da demanda e os padrões de comportamento e interação entre múltiplas variáveis.

## Fonte dos Dados

Os dados foram obtidos através do portal de **Dados Abertos de Curitiba**, uma iniciativa da Prefeitura Municipal para promover a transparência e a inovação.

* **Link para o Dataset:** [Atendimento Médico - E-Saúde](https://dadosabertos.curitiba.pr.gov.br/conjuntodado/detalhe?chave=05954644-5595-4dcb-b961-1e31e22a1c6e)
* **Secretaria Responsável:** Secretaria Municipal da Saúde (SMS)
* **Frequência de atualização:** Mensal

## Principais Insights da Análise Exploratória

A análise revelou diversos padrões e insights sobre a saúde pública na cidade:

* **Sistema de Duplo Foco:** O sistema opera em duas frentes distintas: uma forte base de **Atenção Primária** (UBS), que absorve a maior parte do volume com consultas de rotina, e uma rede de **Urgência** (UPAs), que concentra **100% dos casos** que evoluem para internação.
* **Perfil do Usuário:** O perfil predominante do paciente é **feminino (63%) e adulto**, mas com uma demanda muito significativa de **neonatos (idade 0)**, destacando a importância da saúde pediátrica.
* **Ritmo Operacional Previsível:** A demanda por atendimentos segue padrões semanais e diários claros, com picos de movimento nos dias úteis entre **10h-11h e 14h-16h** e uma queda acentuada nos fins de semana.
* **Curitiba como Polo de Saúde Regional:** A análise geográfica mostrou que a rede de saúde da capital atende a um volume considerável de pacientes de cidades vizinhas, principalmente da Região Metropolitana.
* **Evidências de Determinantes Sociais:** A análise de interação mais profunda encontrou correlações entre **condições de moradia mais precárias** e uma maior proporção de internações por **doenças do aparelho respiratório**, fornecendo uma base de dados para potenciais políticas públicas.

## Estrutura do Notebook

O projeto está contido no arquivo `análise_exploratoria_atendimento_médico_curitiba_v1.1.ipynb` e segue uma estrutura lógica:
1.  **Fase 1: Diagnóstico e Limpeza dos Dados:** Tratamento de valores nulos, remoção de duplicatas e correção de tipos de dados.
2.  **Fase 2: Engenharia de Atributos:** Criação de novas colunas para enriquecer a análise (Idade, Faixa Etária, Turno, Categoria de CID, etc.).
3.  **Fase 3: Análise Exploratória de Dados (EDA):** Uma investigação visual profunda dividida em subseções: Perfil Demográfico, Análise Geográfica, Fluxo de Recursos, Análise Clínica, e Análise de Interações.

## Tecnologias Utilizadas

* **Linguagem:** Python 3
* **Bibliotecas Principais:** Pandas, NumPy, Matplotlib, Seaborn, `ydata-profiling` (para relatório automático), `holidays`.
* **Ambiente:** Jupyter Notebook (executado via VS Code).

## Como Executar o Projeto

1.  Clone este repositório: `git clone https://github.com/seu-usuario/seu-repositorio.git`
2.  Navegue até a pasta do projeto: `cd seu-repositorio`
3.  (Recomendado) Crie um ambiente virtual: `python -m venv .venv` e ative-o.
4.  Instale as dependências: `pip install -r requirements.txt` (Você precisará criar este arquivo. Veja abaixo).
5.  Abra o arquivo `.ipynb` no VS Code ou Jupyter Lab e execute as células em ordem.

Para criar o arquivo `requirements.txt`, use o comando `pip freeze > requirements.txt` no seu terminal com o ambiente ativado.

## Próximos Passos

A base de dados e os insights gerados nesta EDA formam a fundação perfeita para a próxima fase: a **construção de modelos preditivos** para prever o volume de atendimentos, surtos de doenças e risco de internação.

## Autor

**Igor Fiori**
