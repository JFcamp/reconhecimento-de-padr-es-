# reconhecimento de padrões
Autores: Bianca Panacho, Pedro Campos e Vinícius Barbosa.

Esse projeto foi realizado com a linguagem Python, utilizando o altoritmo Random Forest implementado da biblioteca scikit-learn, também utilizamos uma extensão do Visual Studio Vode, Jupyter, para transformar o dataset "parquet" em "csv" e visualizar os dados de forma organizada em formato de tabela.

⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️⚠️

### Aplicação e comparação da rede neural com randow florest.🚀
Optamos pela Random Forest devido à sua destacada interpretabilidade, robustez a hiperparâmetros, capacidade de lidar eficazmente com dados pequenos ou ruidosos, treinamento mais eficiente, menor exigência de normalização intensa e resistência inerente ao overfitting. Esta escolha foi fundamentada na adaptação superior deste modelo ao conjunto de dados fornecido, alinhando-se de maneira mais precisa às necessidades específicas do problema em questão.

## Modelo Escolido:
+ Nome
  Randow florest 
+ Descrição
Random Forest é um algoritmo de aprendizado de máquina que cria múltiplas árvores de decisão e combina suas previsões para melhorar a precisão na classificação. Cada árvore "vota" na classe, e a classe mais votada se torna a predição final. Exemplo: classificação de e-mails como spam ou não spam.
+ Acuracia alcançada
  Utilizando o modelo no data-set fornecido conseguimos uma acuracia de 74% 

## Rede Nueral:
+ Nome
Rede Neural MLP
+ Descrição
Uma Rede Neural MLP (Multilayer Perceptron) é um modelo de aprendizado profundo que consiste em camadas de neurônios conectados. Usada para classificação, ela aprende padrões complexos nos dados durante o treinamento, sendo eficaz em problemas como reconhecimento de imagem, previsões financeiras, etc. Exemplo: classificação de dígitos escritos à mão em um conjunto de dados MNIST.
+ Acuracia alcançada
  Utilizando o modelo no data-set fornecido conseguimos uma acuracia de aproximadamente 72% 

## Como implementar a Rede Neural:

Passo 1: Carregar Bibliotecas e Dados 🔧

Comece importando as bibliotecas necessárias, como pandas, scikit-learn, seaborn e matplotlib. Em seguida, carregue seus dados a partir de um arquivo, por exemplo, usando pd.read_parquet.
- pandas
- scikit-learn
- numpy
- seaborn
- matplotlib
  
Passo 2: Pré-processamento dos Dados ⚙️

Separe suas características (features) e a coluna alvo do conjunto de dados. Divida os dados em conjuntos de treinamento e teste usando train_test_split. Padronize os dados para garantir que todas as características estejam na mesma escala.

Passo 3: Treinamento da Rede Neural MLP com Busca em Grade 🏋️‍♂️

Defina os hiperparâmetros que deseja testar para sua MLP, como o tamanho das camadas ocultas e a taxa de aprendizado. Use a busca em grade (GridSearchCV) para encontrar os melhores hiperparâmetros com base no desempenho nos dados de treinamento.

Passo 4: Ensemble de Modelos com Votação Suave 🤝✨

Crie um ensemble usando o método VotingClassifier. Adicione o modelo MLP com os melhores hiperparâmetros ao ensemble. Treine o ensemble com os dados de treinamento.

Passo 5: Avaliação do Ensemble 📊✅

Faça previsões no conjunto de teste usando o ensemble e avalie sua acurácia usando métricas como accuracy_score.

Passo 6: Visualização de Resultados (Opcional) 📈🔍

Se desejar, você pode visualizar os resultados. Por exemplo, crie uma matriz de confusão para a MLP e, opcionalmente, uma curva ROC para avaliar o desempenho do modelo.


Lembre-se de tornar seu código limpo, legível e bem documentado para facilitar a compreensão.

## Como implementar Randow Florest:


Passo 1: Importar Bibliotecas e Carregar Dados 🌲
Comece importando as bibliotecas necessárias, como pandas e scikit-learn. Carregue seus dados a partir de um arquivo usando, por exemplo, pd.read_parquet.
- pandas
- scikit-learn
- numpy
- seaborn
- matplotlib

Passo 2: Pré-processamento dos Dados 📊

Separe as características (features) e a coluna alvo do conjunto de dados. Divida os dados em conjuntos de treinamento e teste usando train_test_split. Realize qualquer pré-processamento necessário.

Passo 3: Treinamento da Random Forest 🚀

Crie um modelo de Random Forest usando RandomForestClassifier. Ajuste o modelo aos dados de treinamento para permitir que ele aprenda padrões no conjunto de treinamento.

Passo 4: Avaliação do Modelo 🧐

Faça previsões no conjunto de teste e avalie o desempenho da Random Forest usando métricas como acurácia, matriz de confusão e curva ROC.

Passo 5: Visualização dos Resultados (Opcional) 📈

Opcionalmente, crie visualizações para entender melhor os resultados. Pode incluir a visualização da importância das características ou uma representação gráfica da árvore de decisão.

## Tecnologia Usadas:

<table>
  <tr>
    <td>LINGUAGENS</td>
    <td>BIBLIOTECAS</td>
    <td>AMBIENTE DE DESENVOLVIMENTO </td>
  </tr>
  <tr>
    <td>PYTHON</td>
    <td>pandas,scikit-learn
,numpy,seaborn,matplotlib</td>
    <td>VS Code</td>
    
  </tr>
</table>

## Como executar as aplicações:

+ Executando a Aplicação: Rede Neural (MLP)
1) Instalação de Dependências:
Certifique-se de ter as bibliotecas necessárias instaladas. Você pode instalar as dependências executando:
pip install pandas scikit-learn numpy seaborn matplotlib

2) Executando o Código:

Abra o arquivo que contém o código da Rede Neural (MLP).
Execute o script utilizando um ambiente Python.

+Observações Importantes:
Certifique-se de ter um ambiente Python configurado.
Algumas aplicações podem exigir dados específicos ou configurações adicionais. Certifique-se de entender os requisitos específicos de cada aplicação

+ Executando a Aplicação: Random Forest
1) Instalação de Dependências:
Certifique-se de ter as bibliotecas necessárias instaladas. Você pode instalar as dependências executando:
pip install pandas scikit-learn numpy seaborn matplotlib

2) Executando o Código:
   
Abra o arquivo que contém o código da Random Forest.
Execute o script utilizando um ambiente Python.

+Observações Importantes:
Antes de executar, verifique se você possui um conjunto de dados disponível ou ajuste o código para carregar seus próprios dados.
Certifique-se de compreender os hiperparâmetros definidos no código e ajuste conforme necessário, dependendo do seu problema específico.
Avalie a necessidade de ajustar outros parâmetros, como a estrutura da rede neural, de acordo com a complexidade do seu problema.

<center><img src="https://user-images.githubusercontent.com/38620899/106393900-5aa85880-63d8-11eb-88f1-07ac30adad80.gif"></center>

