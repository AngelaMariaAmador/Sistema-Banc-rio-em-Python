# Sistema-Bancario-em-Python
Este projeto implementa um sistema bancário simples utilizando Python. O sistema permite realizar operações básicas como depósitos, saques e a visualização de extratos. Além disso, possui funcionalidades de controle de limite diário de saques e registro detalhado das transações.

## Funcionalidades

- **Depósito**: Permite ao usuário depositar valores na conta, com verificação para evitar depósitos negativos.
- **Saque**: Permite ao usuário realizar saques, respeitando o limite de três saques diários de até R$500 cada.
- **Extrato**: Exibe o extrato das transações realizadas e o saldo atual da conta.
- **Menu Interativo**: Interface de menu para facilitar a interação com o sistema.

## Como Usar

1. Clone este repositório:
    ```bash
    git clone https://github.com/seu-usuario/nome-do-repositorio.git
    ```
2. Acesse o diretório do projeto:
    ```bash
    cd nome-do-repositorio
    ```
3. Execute o script Python:
    ```bash
    python nome_do_arquivo.py
    ```

## Exemplo de Uso

```python
# Teste do Sistema:
conta = Banco()

# Testando Depósito
conta.depositar()  # Solicita ao usuário informar o valor dos depósitos

# Testando Saques
conta.sacar(500)  # Primeiro saque de R$500
conta.sacar(500)  # Segundo saque de R$500
conta.sacar(500)  # Terceiro saque de R$500
conta.sacar(500)  # Tentativa de quarto saque, que deve ser bloqueada

# Visualizando Extrato
conta.visualizar_extrato()  # Mostra o extrato, saldo atual e todos os depósitos
