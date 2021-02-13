### Múltiplos Arquivos
São apresentados conceitos quanto ao tratamento de múltiplos arquivos ao se utilizar uma pasta como fonte de dados:
- É possível introduzir filtros para que apenas arquivos de interesse sejam carregados no Power BI após serem introduzidos na pasta (terminados em csv, por exemplo);
- É importante tomar nota de que o Power Query realiza algumas ações automaticamente que podem introduzir erros. Por exemplo, a tipagem de dados utiliza o nome da
coluna como forma de realizar a operação. Ao tratar vários arquivos de uma vez, as colunas podem apresentar diferentes nomes e, portanto, apresentar alguma 
divergência. No exemplo da aula, algumas colunas apresentavam a data no formato "Agosto 2017", alterando o valor do ano a depender do arquivo;
- Foram introduzidas ferramentas de conversão de linhas em colunas para adaptar documentos do excel para um formato mais condizente com o Power BI. Em outras
palavras, informações no excel tendem a crescer horizontalmente, com a adição de novas colunas para indicar novos meses ou anos, por exemplo. Por outro lado, dados
no Power BI tendem a crescer para baixo;
