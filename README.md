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
