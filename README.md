### Viés Sistêmico em Vistos de Trabalho no Brasil: uma Análise com Regressão Logística e Estatística Inferencial

## Histórico do projeto

  Na primeira atualização de escopo desse projeto foi feita a expansão do objetivo inicial do trabalho para abarcar os conhecimentos adquiridos no curso citado, assim como a criação da pergunta guia do projeto e alguns dos parâmetros de saída e entrada do sistema.

  Na segunda atualização, há especificação sobre a parte estatística do projeto com a definição das variáveis dependentes e independentes e a melhoria geral da organização e estrutura do projeto.

  Nessa terceira atualização, é feito o preenchimento dos parâmetros da primeira etapa da investigação.

## Etapa 1 - Problema de Pesquisa, Mapeamento e Hipóteses
Pergunta de Pesquisa e Escopo

  Este é um projeto educativo em fase de desenvolvimento acerca de vieses sistêmicos na concessão de vistos de trabalho no Brasil e visa utilizar os conhecimentos e dados obtidos no curso Introdução ao R para Análise de Dados de Imigração — SEMUNI 2026 para produzir um painel interativo focado em buscar evidências quantitativas de discriminação racial ou geográfica no deferimento de vistos de trabalho através do uso de estatística inferencial

  Serão analisados exclusivamente os resultado definitivos "Deferido" e "indeferido" - Outros status intermediários ou administrativos como "Em exigência", "cancelado" serão desconsiderados para os propósitos desta pesquisa. 

## Tradução Operacional(Mapeamento das váriaveis)
  A probabilidade de deferimento será calculada usando a função da regressão logística. Nossa variável dependente Y assumirá um valor estrito onde: 0 é indeferido e 1 é deferido.

  Nossas variáveis de interesse ($_$, $_$, $_$) são o fator bloco geopolítico, continente e matriz demográfica predominante de origem da pessoa aplicante e nossa categoria de referência será o continente europeu / Norte Global / Matriz demográfica predominante branca, por representar um grupo privilegiado no contexto migratório.(Para evitar problemas de multicolinearidade, as variáveis serão testadas separadamente)

Variáveis de controle: escolaridade do solicitante($_$), IDH ou Renda per capita do país de origem(váriavel correlacionada, portanto apenas uma das duas)($_$), IDH-M ou Renda per capita do Estado de origem do local de destino($_$), Norma jurídica($_$)

* $X_4$ - Está controlando a influência do fator educacional (capital humano)
* $X_5$ - Está controlando a influência do fator econômico ou social do aplicante (Vulnerabilidade social/econômica de origem)
* $X_6$ - Está controlando a influência do fator econômico ou social do Estado de Destino (demanda do mercado local)
* $X_7$ - Está controlando a influência do fator legal/burocrático (Normas jurídicas / Amparo legal do visto)

## Formalização de hipóteses

A hipótese Nula ($H_0$) é que qualquer tipo de desvio ocorra por pura coincidência ou por variância natural dos dados escolhidos.

A hipótese alternativa ($H_1$) é que isso ocorra por conta de um víes sistêmico contra determinadas matrizes populacionais ou/e blocos geopolíticos. A hipótese $H_0$ só será rejeitada caso o p-valor associado as variáveis de interesse seja menor que 0,05 e o Odds Ratio (OR) gerados sejam significativamente diferentes de 1.

## Governança 

  Os dados pessoais dos aplicantes já estão anônimos em conformidade com a LGPD e a LAI.

  Este é um trabalho acadêmico, independente e autoral, sem vínculo formal com o OBMigra ou do orgão que publicizou a fonte dos dados.

## Métricas de validação

AIC / BIC (para comparação de modelos);
Pseudo-$R^2$ (McFadden);
Matriz de Resíduos / Teste de Hosmer-Lemeshow (ajuste do modelo).

## Etapa 2 - Coleta e ETL:

## Etapa 3 - Análise Exploratória de Dados:

## Etapa 4 - Modelagem Estatística:

## Etapa 5 - Avaliação e Validação:

## Etapa 6 - Divulgação dos dados:



