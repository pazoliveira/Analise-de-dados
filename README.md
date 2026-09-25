### Análise de dados usando R e Shiny para explorar base de dados de Imigração no Brasil

Este é um projeto educativo em fase de desenvolvimento acerca de vieses sistêmicos contra migrantes no Brasil e visa utilizar os conhecimentos e dados obtidos no curso Introdução ao R para Análise de Dados de Imigração — SEMUNI 2026 para produzir um painel interativo focado em buscar evidências quantitativas de discriminação racial ou geográfica no deferimento de vistos de trabalho de migrantes no Brasil através do uso de estatística inferencial

### Histórico do projeto

Na primeira atualização de escopo desse projeto foi feita a expansão do objetivo inicial do trabalho para abarcar os conhecimentos abarcados no curso citado, assim como a criação da pergunta guia do projeto e alguns dos parâmetros de saída e entrada do sistema.

Na segunda atualização, há especificação sobre a parte estatística do projeto com a definição das variáveis dependentes e independentes e a melhoria geral da organização e estrutura do projeto para um projeto de ciência de dados.

### A pergunta que desejamos responder: 

Se temos dois pessoas aplicando para um visto de trabalho no Brasil que possuam a mesma escolaridade, aplicando pela mesmo norma jurídica e indo para o mesmo local, mas de origens ou matrizes demográficas diferentes, isso afeta a chance de deferimento do visto?

### Formulação Estátistica:

Variável dependente: A decisão sobre a concessão do visto(Deferido ou indeferido)

Variáveis independentes: Matriz demográfica predominante de origem(X¹), bloco geopolítico(X²), escolaridade do solicitante(X³), IDH ou Renda per capita do país de origem(váriavel correlacionada, portanto apenas uma das duas)(X⁴), IDH-M ou Renda per capita do Estado de origem do local de destino(X⁵), Norma jurídica(X⁶)

### ETAPAS DO PROJETO:

1ª etapa - Estruturação
Nesta etapa, estrutura-se a arquitetura e organização do projeto, com a definição e explicação educativa sobre os parâmetros de entrada e saída da aplicação.

2ª etapa - Aplicação

Desenvolvimento da aplicação

Organização dos arquivos

Mapeamento

Modelagem estatística

3ª etapa - Finalização
Observam-se os resultados, tiram-se conclusões, revisa-se e compartilha-se o projeto.

### ENTRADAS SELECIONADAS:

Com base nas informações disponíveis no banco de dados, os parâmetros escolhidos para a composição do projeto serão os seguintes:

ALTERNÂNCIA DE PANORAMA (Seletor de visão):
MATRIZ DEMOGRÁFICA PREDOMINANTE DO PAÍS DE ORIGEM

BLOCO GEOPOLÍTICO (Sub-regiões do Sul Global e Norte Global)

FILTROS DE ORIGEM
Matriz Demográfica Predominante:
Checkboxes para seleção individual ou múltipla das 4 matrizes (Asiática, Afrodescendente, Caucasiana ou Povos Originários).

Concentração Populacional:
Slider com o intervalo percentual do grupo no país de origem.

Perfil Econômico:
Faixa de renda do Banco Mundial e IDH.

FILTROS DE DESTINO
UF / Região de Recepção:
Seleção dos estados de destino pela coluna de localização do estrangeiro.

Perfil Socioeconômico do Destino:
PIB per capita e IDH-M das Unidades Federativas brasileiras.

FILTROS INSTITUCIONAIS:
Amparo Legal / Norma Jurídica (Resoluções Normativas e Portarias):
Diferentes normas possuem diferentes requisitos e exigências legais.

Modalidade Administrativa (CGIL vs. CNIg):

CGIL (Coordenação-Geral de Imigração Laboral): analisa pedidos ordinários.

CNIg (Conselho Nacional de Imigração): analisa casos mais complexos e recursos.

Perfil do Solicitante:
Escolaridade, faixa etária e gênero.

PARÂMETROS DE SAÍDA (Métricas exibidas):
Taxa Bruta de Indeferimento (%)

Risco Relativo Ajustado (Odds Ratio da Regressão Logística)

### Fonte dos Dados e Governança
* **Origem:** Observatório das Migrações Internacionais (OBMigra) / Ministério da Justiça e Segurança Pública (MJSP) / Ministério do Trabalho e Emprego (MTE).
* **Licenciamento:** Dados Abertos (Lei nº 12.527/2011 e Decreto nº 8.777/2016).
* **Proteção de Privacidade:** A base utilizada é integralmente anonimizada, não contendo dados pessoais identificáveis (PII), em conformidade com a LGPD (Lei nº 13.709/2018).
* **Aviso de Isenção (Disclaimer):** Este projeto é uma análise independente com fins acadêmicos/estudantis e não possui vínculo oficial com o Ministério do Trabalho e Emprego ou com o OBMigra.

