<h1>SUMÁRIO:</h1>
<li>   1. Objetivos do projeto</li>
<li> 2. Sobre os dados utilizados</li>
<li>3. Explicando a ineficácia dos algoritmos</li>
<h2>1. Objetivos do Projeto</h2>
O projeto Classificador de Arritmias visava obter um algoritmo capaz de analisar dados de
um eletrocardiograma e prever o diagnóstico de um paciente.
2. Sobre os dados utilizados
Os dados utilizados podem ser encontrados em:
https://www.kaggle.com/datasets/bulentesen/cardiac-arrhythmia-database
O dataframe em questão contia 279 colunas, porém grande parte delas foi eliminada por não
haver significado explicado pelo autor dos dados. Somente as seguintes características
foram utilizadas: Idade, Sexo, Altura, Peso, Duração qrs, intervalo PR, intervalo QT, Intervalo
T, Intervalo Q, qrs, T, P, QRST, frequência cardíaca, onda q, onda r, onda s, onda R’ e Onda
S’.
Os diagnósticos foram separados em 16 categorias, indicadas de 1 a 16.
Dessa forma:
01 Normal
02 Ischemic changes (Coronary Artery Disease)
03 Old Anterior Myocardial Infarction
04 Old Inferior Myocardial Infarction
05 Sinus tachycardy
06 Sinus bradycardy
07 Ventricular Premature Contraction (PVC)
08 Supraventricular Premature Contraction
09 Left bundle branch block
10 Right bundle branch block
11 1. degree AtrioVentricular block
12 2. degree AV block
13 3. degree AV block
14 Left ventricule hypertrophy
15 Atrial Fibrillation or Flutter
16 Others
O dataset apresentava inicialmente 452 valores porém após o tratamento de dados faltantes
que foi necessário para não prejudicar a previsão, foi possível utilizar apenas 420 valores.
3 – Explicando a Ineficácia dos algoritmos
O baixo número de dados (420) alinhado ao alto número de características (19)
impossibilitou uma boa atuação dos algoritmos de inteligência artifical. Foram testados, 4
deles. Regressão Linear, Árvore de Decisão, Random Forest e Redes neurais. Os algoritmos
que melhor performaram foram o de Random Forest, que teve em torno de 66.67 % de
acurácia, Redes neurais com em torno de 65 % de acurácia e SVC com em torno de 60%.
Para a utilização na área da saúde, algoritmos com esse nível de acurácia são irrelevantes
</body>
</html>
