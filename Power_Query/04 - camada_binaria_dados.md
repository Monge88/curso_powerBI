### Camada binária e de dados
Algumas informações pertinentes de um arquivo de dados podem estar presentes em seu nome. No exemplo dado nesta aula, os arquivos eram nomeados no formato
"Ana Clara - 2017.txt", ou seja, o nome de uma pessoa e o ano correspondente às suas atividades monetárias estão na camada binária. Tais informações precisam ser
transferidas para a camada de dados. A imagem a seguir mostra a área de trabalho do Power Query após obter dados de uma pasta que contém os arquivos a serem 
trabalhados. Clicar em *binary* exibe os dados referentes a cada arquivo. A ideia, portanto, é inserir os dados da coluna "Name" em cada um dos arquivos *binary*.

![](https://github.com/Monge88/curso_powerBI/blob/main/figure/ex4.png)

Ao se clicar no ícone no canto superior direito da imagem, "Combinar arquivos", o Power Query irá realizar uma série de etapas para combinar os arquivos, tais como
expandir tabelas, alterar tipos etc, como mostra a figura a seguir.

![](https://github.com/Monge88/curso_powerBI/blob/main/figure/ex5.png)

A etapa "Invocar Função Personalizada1" em particular extrai os dados de cada *Binary* e os armazena no objeto *Table*, como mostra a figura a seguir.

![](https://github.com/Monge88/curso_powerBI/blob/main/figure/ex6.png)

Dessa forma, basta apenas excluir os passos subsequentes e também a coluna com os objetos *binary*, já que os dados necessários estão no o objeto *Table*. Após isto,
basta clicar no ícone no canto superior direito da imagem, "Expandir", para que os dados sejam então atribuídos a cada valor da coluna "Name". As transformações
subsequentes são triviais e já realizadas em aulas anteriores.
