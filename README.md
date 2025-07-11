# ML_Rogerio
# 1. Preparação dos Dados
O primeiro passo do projeto foi a preparação dos dados, uma etapa essencial para garantir a qualidade da análise. O processo de limpeza e organização incluiu as seguintes ações:
Carga dos Dados: O dataset foi importado de uma fonte online.
Limpeza dos Nomes das Colunas: Espaços em branco foram removidos para evitar erros.
Conversão de Tipos: Datas foram ajustadas para o formato datetime e valores monetários para o formato numérico (float).
Tratamento de Valores Ausentes: Descrições de bens que estavam vazias foram preenchidas com "Desconhecido".
Remoção de Outliers: Bens com valores muito acima da média foram removidos para não distorcer a análise.
Criação de Features: Novas colunas, como Ano_Atual e Tipo_Cod (código numérico para o tipo de bem), foram criadas para ajudar na modelagem.
Com isso, o dataset ficou pronto para a próxima fase.

2. Análise Exploratória dos Dados
Com os dados limpos, a próxima fase foi explorar as informações para entender melhor o patrimônio dos candidatos.

2.1. Maiores Patrimônios Declarados
Foi feito um ranking dos candidatos por patrimônio total para verificar a concentração de riqueza.
O gráfico mostra que poucos candidatos (identificados por seu ID) concentram a maior parte do patrimônio, o que é um dado importante sobre o perfil econômico deles.

2.2. Análise por Tipo de Bem
Aqui, a ideia foi ver quais tipos de bens são mais valiosos no geral.
Os gráficos mostram que os bens com maior valor total não são necessariamente os mesmos com maior valor médio. Isso ajuda a entender quais bens são mais valiosos individualmente.

2.3. Distribuição Geográfica do Patrimônio
A análise final foi sobre a soma do patrimônio por estado (UF).
O gráfico mostra a concentração do patrimônio declarado por estado, indicando diferenças regionais.

3. Modelagem Preditiva
Nesta fase, o objetivo foi criar um modelo para prever o valor de um bem (VR_BEM_CANDIDATO) usando o ano da declaração e o tipo do bem como base. Os dados foram divididos em 80% para treino e 20% para teste, e as variáveis foram padronizadas com StandardScaler.

Foram testados dois modelos:
Regressão Linear
Random Forest Regressor


Este projeto cobriu as principais etapas com dados. Após a limpeza, a análise exploratória mostrou informações úteis sobre a riqueza dos candidatos. Em seguida, a parte de modelagem testou dois algoritmos, onde o Random Forest se mostrou mais eficaz para prever o valor dos bens. O trabalho mostrou na prática como usar dados para encontrar padrões e fazer previsões
