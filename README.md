# 📊 Análise Exploratória de Dados (EDA) — Sinistros de Trânsito em Alagoas (RENAEST)

Este projeto realiza uma Análise Exploratória de Dados (EDA) focada na gravidade, comportamento espacial e dinâmicas de coleta de sinistros de trânsito ocorridos no estado de Alagoas, utilizando Python e dados unificados do **RENAEST** (Registro Nacional de Sinistros e Estatísticas de Trânsito).

Nota de Qualidade do Dado: Os dados analisados apresentam inicialmente 154 óbitos registrados sob o ano de referência de 2025 na base unificada do RENAEST. Contudo, estatísticas locais consolidadas pelo DETRAN Alagoas apontam um total de 447 óbitos no mesmo período anual, indicando uma janela importante de defasagem de sincronização entre o relatório federal e o dataset público. (IMPORTANTE RESSALTAR QUE O DATASET É ALIMENTADO APENAS ATÉ SETEMBRO DE 2025)

---

### 🚀 Tecnologias Utilizadas

Python 
Pandas: Limpeza, filtragem e manipulação de dados estruturados.
Matplotlib: Construção de subplots e visualizações gráficas avançadas.

---

🔍 Principais Descobertas e Insights da Análise

Abaixo estão as respostas para as perguntas de negócio e impacto social que guiaram esta análise exploratória:

### 1. Qual é a letalidade real dos sinistros por período do dia?
**Resposta:** Ao cruzar o volume total de acidentes com o somatório de óbitos, os dados provam que, embora os períodos da **Tarde, Noite e Manhã** concentrem o maior volume absoluto de acidentes, a **Madrugada** é proporcionalmente a fase do dia mais letal, registrando a maior taxa de letalidade por sinistro.

### 2. Quais são os principais comportamentos ou fatores que geram acidentes fatais?
**Resposta:** Através da distribuição das causas, identifica-se de forma clara que as falhas humanas comportamentais estão no topo das causas de morte em sinistros, destacando-se a **"Falta de atenção do condutor"** e a **"Desobediência às normas de trânsito pelo condutor"**.

### 3. Qual é o nível de subnotificação ou ausência de dados sobre as causas dos acidentes?
**Resposta:** A análise visual revela de forma preocupante que o indicador **"Sem informação"** é a barra mais longa do gráfico de causas fatais. Isso evidencia um problema crítico de completude na coleta primária e preenchimento dos boletins que alimentam o RENAEST.

### 4. Quais os aspectos notados e as diferenças na forma de coletar os registros de acidentes entre Maceió e Arapiraca?
**Resposta:** No dataset trabalhado, Arapiraca possui uma quantidade expressivamente maior de sinistros registrados em comparação com a capital, Maceió. Esta diferença volumétrica acentua discussões metodológicas sobre o fluxo de trabalho de coleta:
* **Maceió (Predomínio de Dispositivos Eletrônicos):** O uso de meios digitais costuma gerar dados mais padronizados e estruturados. Contudo, sistemas eletrônicos rígidos ou com excesso de campos obrigatórios podem desencorajar o registro de pequenos incidentes, priorizando apenas ocorrências graves e gerando subnotificação de sinistros leves. Isso pode mascarar uma falsa sensação de "modernização e redução de acidentes".
* **Arapiraca (Predomínio de Blocos de Papel):** O tradicional bloco de notas em papel é extremamente portátil, ágil no local do acidente e independente de sinal de internet ou baterias ("não trava"). Essa facilidade operacional pode explicar o volume tão alto de ocorrências capturadas no município. Por outro lado, o papel abre margem para dados ilegíveis ou campos em branco, alimentando diretamente a alta taxa de registros "Sem informação".

---

## 🛠️ Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)
