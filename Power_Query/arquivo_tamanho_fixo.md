### Arquivos de tamanho fixo
São um tipo especial de arquivo, normalmente com formato txt, onde as colunas estão separadas por espaços. No momento da leitura do arquivo, não é possível fazer a 
separação das colunas e resta à etapa de tratamento de dados corrigir isto. A figura a seguir mostra a configuração do arquivo já lido pelo Power Query. 

![](https://github.com/Monge88/curso_powerBI/blob/main/figure/ex3.png)

Uma alternativa para separar as colunas é utilizar a ferramenta "dividir coluna -> por posições", onde deve ser informado a posição do início de cada coluna onde
a divisão deve ocorrer. Caso não haja um arquivo de *schema* que forneça as informações pertinentes do arquivo em questão, um editor de texto como o notepad++ pode
ser usado para determinar as posições de separação. Subsequentes filtragem dos dados são então suficientes para deixar o arquivo pronto para que as colunas sejam 
tipadas e então carregadas no Power BI.

*Nota:* Podem haver inconsistências entre a língua do programa e dos arquivos sendo analisados. Por exemplo, neste arquivo em específico, a coluna com datas e 
valores monetários estavam em formatação inglesa, enquanto o Power BI que uso está em português. Dessa forma, o Power Query apresentou erro na hora de tipar estas
colunas. Uma alternativa para conseguir tipar as colunas neste tipo de ocasião é *botão direito na coluna -> Alterar Tipo -> Usando a Localidade...*. Aqui é 
escolher a tipagem da coluna e em qual formatação de localidade ela está atualmente. Neste exemplo foi necessário selecionar a opção *Inglês (Estados Unidos)*.
