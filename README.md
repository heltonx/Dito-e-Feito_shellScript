# Dito-e-Feito_shellScript
De modo análogo aos Katas no Karatê, os Dito-e-Feitos são sequências de atividades visando exercitar o conhecimento em uma determinada tecnologia, do comando mais simples até uma arquiteturação mais complexa, visando melhorar os reflexos no desempenho e na memorização da tecnologia. 

O Dito-e-Feito a seguir vai do simples ao complexo na prática do shell script, com foco em TERMUX. É baseado nas aulas práticas no Termux com o amigo "Free"

================================================================

Item 1
aquecimento
diferença entre o nano (e outros editores de texto) e o touch
echo "texto"
echo dentro de um arquivo:
echo texto123 > arquivoTeste
abrir arquivo:
cat arquivoTeste

em resumo:
echo vai escrever
o > vai jogar dentro de algum arquivo
o cat serve pra ver o conteudo

================================================================

Item 2
função básica
minha_funcao () { echo "sou uma função"; "por hoje é só";}

-Como executar a função:
minha_funcao

================================================================

Item 3

first:
-touch arquivo
-nano arquivo

#COPY CODE FROM HERE
#!/bin/bash
#Purpose: Dito-e-Feito Shell Script Termux Item 3 - Somar e diminuir (plus and minus)
#Created date Mon Jan 8 21:24 2024
#Author: Mr Terceiro (but code strong inspired on Mr Rumar code, check the yellow notebook)
#Start
echo -e "Enter first value: \c"
read -r a
echo -e "Enter second value: \c"
read -r b

echo "addition values expr $a + $b"
echo "minus values expr $a - $b"

echo "Completed Successfully"
echo  "END"
#END OF THE CODE TEXT

chmod 777 arquivo (dont do the 777 command everytime, but just in this case)
./arquivo

================================================================

Item 4
Understanding difference between quotation marks

first:
-touch arquivo
-nano arquivo

#COPY CODE FROM HERE
#!/bin/bash
#Purpose: Dito-e-Feito Shell Script Termux Item 4 - Difference between quotation marks (Sintax explanation)
#Created date Mon Jan 11 15:47 2024
#Author: Mr Terceiro (but code strong inspired on someone code, check the yellow notebook)
#Start

VAR1=123
VAR2=ABC

#Double quotes (Variables values shown between strings)
echo "Execute double quotes $VAR1 $VAR2"

#Single quotes ("Force" the print of the strings, in other words, just will print the variable names)
echo 'Execute single quotes $VAR1 $VAR2'

#Reverse quotes (comands between strings)
echo "This hostname is: `hostname`"

#End#
#END OF THE CODE TEXT

chmod 777 arquivo (dont do the 777 command everytime, but just in this case)
./arquivo

================================================================

Dito 5

-Create a file called countargs.sh

#COPY CODE FROM HERE
#! /bin/bash
#Purpose: Counting given positional parameters
#Start
echo "You current given parameters are: $#"

#END OF THE CODE TEXT

-Execute at your bash the following command:

$ sh countargs.sh hi I Am Tonho
