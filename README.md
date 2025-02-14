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

  
