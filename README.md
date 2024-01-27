# Manipulating_data_with_python_Challenge

## Esse é o Desafio técnico da Tunts.Rocks.

## A proposta é a seguinte: 
Criar uma aplicação em uma linguagem de programação de sua preferência (caso esteja se  candidatando a uma vaga de linguagem de programação específica, exemplo: programador  node.js, utilizar a linguagem/tecnologia específica da vaga). A aplicação deve ser capaz de ler  uma planilha do google sheets, buscar as informações necessárias, calcular e escrever o  resultado na planilha. 

No meu caso eu optei por utilziar o python, já que é uma linguagem excelente para manipulação de dados. 

## Linha de pensamento:
Para desenvolver o programa a primeira coisa que fiz foi separar o meu problema em problemas menores, o que facilita na minha resolução.

1. O primeiro ponto era uma forma de por meio da linha de comando obter o nome da planilha que continha os dados. Para isso utilizei o import sys, e o argv para separar o nome da planilha.

2. O segundo ponto foi abrir a tabela com o uso do openpyxl.

3. Depois eu precisei percorrer linha a linha do meu arquivo aplicando as minhas regras de negócio que são:

             Calcular a situação de cada aluno baseado na média das 3 provas (P1, P2 e P3), conforme a  tabela:
              
              Média (m) Situação:
              
              m<5  - Reprovado por Nota
              
              5<=m<7  - Exame Final
              
              m>=7  - Aprovado
              
              Caso o número de faltas ultrapasse 25% do número total de aulas o aluno terá a situação  "Reprovado por Falta", independente da média.  Caso a situação seja "Exame Final" é necessário calcular a "Nota para Aprovação Final"(naf) de  cada aluno de acordo com seguinte fórmula: 
              
              5 <= (m + naf)/2
              
              Caso a situação do aluno seja diferente de "Exame Final", preencha o campo "Nota para  Aprovação Final" com 0. 
              
              Arredondar o resultado para o próximo número inteiro (aumentar) caso necessário. Utilizar linhas de logs para acompanhamento das atividades da aplicação. 
5. E por fim precisei salvar os dados escritos na tabela.

## Resultado final:
Tabela após a execução do script:
![image](https://github.com/JoseErivan/Manipulating_data_with_python_Challenge/assets/105927510/55f61e98-f767-4fb1-bc97-d06857124a9e)

Respostas do programa no console do sistema operacional:
![image](https://github.com/JoseErivan/Manipulating_data_with_python_Challenge/assets/105927510/373d6653-b458-497e-b1cc-dfa258c91acd)

## Intalações de requisitos para executar o programa:
Para que o programa funcione, primeiro precisamos baixar a biblioteca openpyxl que é uma biblioteca Python para ler/gravar arquivos xlsx/xlsm/xltx/xltm do Excel 2010.

O comando de instalção é: pip install openpyxl. (Lembrando que o python já precisa estar instalado na máquina)

## Como utilizar o programa:
Para utilizar o programa no terminal do sistema operacional vamos digitar o seguinte código:
python + ./script.py + nome_da_tabela_com_os_dados (Remova o sinal de soma) 

O programa vai mostrar informações sobre o funcionamento, inclusive se foi ou não bem sucedido em sua operação.

## É isso!
  Muito obrigado por testar meu programa, se encontrou algum erro ou algo que possa melhorar fique a vontade para compartilhar sua ideia!

José Erivan Ramalho Ferreira Filho






# English version from Readme

## This is the Tunts.Rocks Technical Challenge.

## The proposal is as follows:
Create an application in a programming language of your choice (if you are applying for a position in a specific programming language, example: node.js programmer, use the specific language/technology of the position). The application must be able to read a Google Sheets spreadsheet, search for the necessary information, calculate and write the result in the spreadsheet.

In my case I chose to use Python, as it is an excellent language for data manipulation.

## Line of thinking:
To develop the program, the first thing I did was separate my problem into smaller problems, which makes it easier to solve.

1. The first point was a way to use the command line to obtain the name of the spreadsheet that contained the data. To do this, I used import sys, and argv to separate the name of the spreadsheet.

2. The second point was to open the table using openpyxl.

3. Then I needed to go through my file line by line applying my business rules, which are:

              Calculate the situation of each student based on the average of the 3 tests (P1, P2 and P3), according to the table:
              
               Average (m) Situation:
              
               m<5 - Failed by Grade
              
               5<=m<7 - Final Exam
              
               m>=7 - Approved
              
               If the number of absences exceeds 25% of the total number of classes, the student will have the status "Failed due to Absence", regardless of the average. If the situation is "Final Exam", it is necessary to calculate the "Final Approval Grade" (naf) for each student according to the following formula:
              
               5 <= (m + naf)/2
              
               If the student's status is different from "Final Exam", fill in the "Grade for Final Approval" field with 0.
              
               Round the result to the next whole number (increase) if necessary. Use log lines to monitor application activities.
5. And finally I needed to save the data written in the table.

## Final result:
Table after script execution:
![image](https://github.com/JoseErivan/Manipulating_data_with_python_Challenge/assets/105927510/55f61e98-f767-4fb1-bc97-d06857124a9e)

Program responses in the operating system console:
![image](https://github.com/JoseErivan/Manipulating_data_with_python_Challenge/assets/105927510/373d6653-b458-497e-b1cc-dfa258c91acd)

## Requirements installations to run the program:
For the program to work, we first need to download the openpyxl library which is a Python library to read/write Excel 2010 xlsx/xlsm/xltx/xltm files.

The installation command is: pip install openpyxl. (Remember that Python must already be installed on the machine)

## How to use the program:
To use the program in the operating system terminal, type the following code:
python + ./script.py + table_name_with_data (Remove the sum sign)

The program will show information about its operation, including whether or not it was successful in its operation.

## And that!
   Thank you very much for testing my program, if you found any errors or something that could improve, feel free to share your idea!

José Erivan Ramalho Ferreira Filho
