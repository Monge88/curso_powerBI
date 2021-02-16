### Informações em abas do excel

Alguns arquivos em excel podem separar informações por abas. No exemplo da aula, cada uma das abas do arquivo excel eram utilizadas para fornecer informações sobre
as atividades financeiras de pessoas diferentes, sendo necessário, portanto, unir tais informações em uma única tabela no Power BI. O procedimento para isso é
relativamente simples e envolve o uso do linguagem M. A imagem a seguir mostra a pasta com os arquivos já inseridos no Power Query.

![](https://github.com/Monge88/curso_powerBI/blob/main/figure/ex7.png)

É recomendável duplicar o arquivo original na barra de consultas devido aos próximos passos que serão necessários. A figura a seguir mostra a tela a ser gerada ao
se clicar em *binary* no novo arquivo criado após a duplicação do arquivo original. Em especial, nota-se o comando necessário na linguagem M para realizar este 
passo.

![](https://github.com/Monge88/curso_powerBI/blob/main/figure/ex8.png)

Os dados referentes a cada aba estão contidos no objeto *Table*. Uma forma de adicionar as colunas "Name" e "Data" no consulta original, mostrada na primeira figura,
é o utilizar o comando "Coluna Personalizada" e fornecer o código em M "Excel.Workbook([Content])" copiado da imagem acima. Note que foi necessária a adição dos
colchetes ao redor da palavra "Content" para que o conteúdo de todas as abas fosse recuperado. A figura a seguir mostra o resultado desta operação.

![](https://github.com/Monge88/curso_powerBI/blob/main/figure/ex9.png)

Os passos seguintes já foram cobertos em aulas anteriores e reference a fazer a expansão da coluna "Data" e subsequente tratamento dos dados.
