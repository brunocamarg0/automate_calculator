# Calculadora

# Para executar o arquivo em .sh, você deve criar um script no Power Shell:

Passo 1: Digite no seu Power Shell o comando nano calculadora.sh
Passo 2: Crie um script no qual automatize o executavel da calculadora, segue exemplo abaixo:

#!/bin/bash

# Defina o caminho do script Python
SCRIPT="calculadora.py"

# Verifique se o arquivo existe
if [ -f "$SCRIPT" ]; then
    echo "Executando a calculadora..."
    python3 "$SCRIPT"
else
    echo "Erro: O arquivo $SCRIPT não foi encontrado."
fi

Passo 3: Salve o script através do comando CTRL + X e após script salvo insira comando ./calculadora.sh


# Código em Python

lista = [1,2,3,4,5,6,7,8,9,10] # variável do tipo lista do 1 ao 10
num1 = input ("Digite um número: ") # pegar informação do usuário através do input para adicionar 1 número
operador = input ("Digite o operador (+, -, *, /):") # pegar informação do usuário através do input para adicionar o operador
num1_convert = int(num1) #conversão da variável num1 para inteiro

for i, val in enumerate(lista): # for onde o "i" é o indice da variável lista, o val recebe cada elemento da lista
  if num1_convert >= 11: # se num1 for maior ou igual á 100 inserir print abaixo
    print("Número maior que 10, favor inserir numeração de 0 á 10!")
    break
  elif operador == '+': # se o operador escolhido pelo usuário for + então seguir com print abaixo
      print(num1_convert ,'+', val, '=', num1_convert + val) #num1_convert pega o número inserido pelo usuário insere o + pega o val da condição que começa com 1 e soma com a o valor que é o indice da lista.
  elif operador == '-':# se o operador escolhido pelo usuário for - então seguir com print abaixo
      print(num1_convert ,'-', val, '=', num1_convert - val) #num1_convert pega o número inserido pelo usuário insere o - pega o val da condição que começa com 1 e subtrai com a o valor que é o indice da lista.
  elif operador == '*':# se o operador escolhido pelo usuário for * então seguir com print abaixo
      print(num1_convert ,'*', val, '=', num1_convert * val) #num1_convert pega o número inserido pelo usuário insere o * pega o val da condição que começa com 1 e multiplica com a o valor que é o indice da lista.
  elif operador == '/':# se o operador escolhido pelo usuário for / então seguir com print abaixo
      print(num1_convert ,'/', val, '=', num1_convert / val) #num1_convert pega o número inserido pelo usuário insere o / pega o val da condição que começa com 1 e divide com a o valor que é o indice da lista.



  
