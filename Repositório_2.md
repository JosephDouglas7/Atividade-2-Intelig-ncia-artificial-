### Nome do aluno: Joseph Douglas Moura Batista 
### matrícula: 20230002504   
### Link para o dataset: [dataset](https://colab.research.google.com/drive/1Rf_DMPLYV6OUE8BpiCHFbuPnG7nGkLAj?usp=sharing)   
### Breve descrição do projeto e dos objetivos: 

o dataset contém informações detalhadas sobre pacientes de um hospital.Os problemas que serão trabalhados para a chegada da decisão de qual abordagem de modelagem é mais adequada são valores ausentes, outliers, correlações e visualizações com interpretação e Descrição das técnicas aplicadas e justificativas.  


### Instruções claras de execução:

1. Baixar o dataset: [stroke_risk](https://www.kaggle.com/datasets/mobeenfatimah/stroke-risk-prediction-dataset?resource=download)
2. Entrar no link para o notebook virtual: [notebook virtual](https://colab.research.google.com/drive/1Rf_DMPLYV6OUE8BpiCHFbuPnG7nGkLAj?usp=sharing) 
3. Fazer upload do dataset para o notebook do colab
    
### Resumo dos principais resultados e da tabela comparativa final  

 o desempenho comparativo dos algoritmos Logistic Regression, Random Forest e XGBoost com base em métricas preditivas, eficiência computacional e interpretabilidade. Em termos de desempenho e generalização, todos os modelos empataram com métricas perfeitas de 1,0 e gap zero entre treino e teste; contudo, há um alerta crítico de que resultados perfeitos podem indicar vazamento de dados (data leakage) ou dados triviais, exigindo uma auditoria rigorosa do pipeline antes da produção. No aspecto da eficiência computacional, a Regressão Logística destacou-se como a mais rápida no treinamento (1,61 s), seguida de perto pelo XGBoost (2,23 s), enquanto o XGBoost sobressaiu-se drasticamente no consumo de memória, utilizando apenas 0,38 MB. Além disso, o aprendizado de máquina demonstrou ser incomparavelmente mais eficiente em tempo e esforço em relação à codificação manual de sistemas especialistas baseados em regras. Quanto à interpretabilidade, a Regressão Logística oferece transparência direta por meio de coeficientes, enquanto Random Forest e XGBoost funcionam como "caixas-pretas", exigindo ferramentas auxiliares como o SHAP, o que é mandatório em setores regulados como saúde, finanças ou direito. Por fim, as recomendações práticas apontam o XGBoost como a escolha principal pela excelente combinação de baixo consumo de memória e alta performance, e a Regressão Logística como a alternativa ideal para cenários que exigem transparência jurídica ou clínica direta. 

#### Tabela comparativa final 

modelo| acuracia_treino | acuracia_teste | gap_generalização| f1_score_teste| roc_auc_teste | Tempo_treino_s | tempo_inferencia_ms | uso_memoria_mb 
|------------------|------------|-----------|----------|----------|----------|-----------|----------|----------|
logistic regression| 1.0        | 1.0       | 0.0      |1.0       | 1.0      |1.6082     | 0.0008   | 107.2615 | 
Ramdom Forest      | 1.0        | 1.0       | 0.0      |1.0       | 1.0      |9.4440     | 0.0123   |  16.2140 |  
\XGBoost           | 1.0        | 1.0       | 0.0      |1.0       | 1.0      |2.2253     | 0.0028   |   0.3830 |

