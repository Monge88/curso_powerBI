### Coluna condicional
A ferramenta "coluna condicional" permite adicionar uma coluna que é calculada com base em outras colunas ou em valores fornecidos pelo usuário. Os detalhes para
sua implementação são mostrados na figura a seguir.

![](https://github.com/Monge88/curso_powerBI/blob/main/figure/coluna_condicional.png)

Ela pode ser utilizada, entre outras coisas, para separar dados com tipos diferentes(*strings* e números por exemplo) quando a formatação destes dados impedir opções
mais simples como a "coluna de exemplos". Por exemplo, a figura a seguir mostra uma situação onde a coluna "Mesclado" foi criada com o uso da ferramenta "coluna de 
exemplos". Note que a formatação dos dados fez com *strings* que deveriam pertencer à coluna "Materiais" fossem erroneamente colocadas na coluna "Tempo", devido a
presença de vírgulas. A criação da coluna "Mesclado" foi uma tentativa de corrigir esse erro. No entanto, o Power BI não foi capaz de separar corretamente os valores
e por isso foi necessário o uso da ferramenta "coluna condicional"

![](https://github.com/Monge88/curso_powerBI/blob/main/figure/ex1.png)

Neste caso, para separar corretamente os valores na coluna "Mesclado", a lógica a ser aplicada seria, por exemplo: <br>
*Se "Mesclado" contém ":", então "Materiais"* <br>
*Senão "Mesclado"* <br>
Ou seja, o Power BI irá percorrer as linhas da coluna "Mesclado" e, caso a linha contenha o caractere ":", o valor a ser utilizado nesta linha será o contido na 
coluna "Materiais", do contrário será utilizado o valor da própria coluna "Mesclado". <br>

### Coluna de exemplos
A ferramenta "coluna de exemplos", por outro lado, permite ao usuário fornecer valores para uma coluna de acordo com uma ação que ele deseja que o Power BI 
interprete. Por exemplo, a figura a seguir mostra algumas das colunas do exemplo anterior, "Materiais" e "Tempo". Alguns valores da coluna "Materiais" foram 
inseridos na coluna "Tempo" devido à presenção de vírgulas. Uma alternativa para iniciar o tratamento destes dados é utilizar a ferramenta "coluna de exemplos" e
fornecer os valores na formatação que seria correta, como por exemplo, "Farinha, Chocolate em Pó e Chocolate Granulado". O Power BI deve ser capaz de entender que 
é necessário unir os dados destas duas colunas. O resultado final seria a coluna "Mesclado" da figura no exemplo anterior.

![](https://github.com/Monge88/curso_powerBI/blob/main/figure/ex2.png)
