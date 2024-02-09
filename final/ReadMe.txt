Este projeto está dividido em 10 notebooks, todos corridos no Google colabs, por uma questão simplificação no que toca a dependências, à exceção dos notebooks 8,9 e 10.

Para estes três últimos notebooks será necessário:
 -Ter a seguinte versão do Python: Python 3.9.5
- Instalação do tensorflowO tensorflow: pode ser instalado no próprio Jupyter notebook com !pip install tensorflow.


Em baixo estão enumerados os diferentes Notebooks:


Pre-processamento dos dados e Preparação:
    
    1. ​Data_Pre_Processing: Procede-se à realização do pré processamento dos dados, 

    2. ​Feature_Extraction – Dá-se a extração dos MFCC (Mel-Frequency Ceptral Coefficient); 

​    3. Label_Extraction – Onde ocorre a realização de one-hot encoding das classes e criação dos array 3D; 


Implementação dos classificadores, estruturação e preparação dos dados:


​    4. test_main_functions – Contém todas as funções gerais para uma iteração e para o 10-fold cross validation; 


Definição da arquitetura dos modelos:

    5. ​Architectures – definição da arquitetura das redes neuronais recurrent unidirecional(rnn) e Multi-Layer Perceptron(mlp) 

​    6. Bidirectional_rnn- Treina-se, para uma iteração, a bidirectional recurrent neural network, estando também incorporado a sua arquietura;


Estratégia de treino e avaliação da performance:

​    7. Hyperparameters – Faz-se um teste manual dos diferentes hiperparâmetros.

    8. ​Best_Hyperparameters – Faz-se um teste automatizado de todas as combinações possíveis dos diferentes hiperparâmetros, para a rede neuronal mlp, para uma iteração. Usa-se o TensorBoard.

    9. ​Individual_Best_Hyperparameters- Dá-se a automatização dos hiperparâmetros de forma individual, isto é, a cada hiperparâmetro é lhe atribuído 3 valores possíveis que pode tomar.
                                        Os parâmetros são então individualmente "isolados" numa lista para que lhe sejam atribuídos esses valores e, os restantes, mantém o valor atribuído como termo de comparação.
                                        Usa-se o TensorBoard e a mlp.

                                        

    10. ​Robustness – Efetua-se a avaliação da robustez das redes neuronais, para uma iteração.