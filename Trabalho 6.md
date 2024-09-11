**Exercício 1**

def imprimir_informacoes(nome, idade, cidade):
    # Usando print com sep e end para formatar a saída
    print(f"Nome: {nome}", end=" - ")
    print(f"Idade: {idade}", end=" - ")
    print(f"Cidade: {cidade}!")

# Exemplo de uso
if __name__ == "__main__":
    imprimir_informacoes("Julia", 23, "Rio de Janeiro")




**Exercício 2**
def calculadora():
    # Solicita ao usuário o primeiro número
    num1 = float(input("Digite o primeiro número: "))
    # Solicita ao usuário o segundo número
    num2 = float(input("Digite o segundo número: "))
    # Solicita ao usuário a operação desejada
    operacao = input("Digite a operação desejada (+, -, *, /): ")
    
    # Verifica a operação e calcula o resultado
    if operacao == '+':
        resultado = num1 + num2
    elif operacao == '-':
        resultado = num1 - num2
    elif operacao == '*':
        resultado = num1 * num2
    elif operacao == '/':
        if num2 == 0:
            print("Erro: Divisão por zero não é permitida.")
            return
        resultado = num1 / num2
    else:
        print("Operação inválida. Por favor, escolha +, -, * ou /.")
        return
    
    # Imprime o resultado da operação
    print(f"O resultado de {num1} {operacao} {num2} é: {resultado}")

# Exemplo de uso
if __name__ == "__main__":
    calculadora()




**Exercício 3**
def listar_compras():
    # Solicita ao usuário para digitar os itens separados por vírgula
    entrada = input("Digite os itens da lista de compras separados por vírgula: ")
    
    # Divide a entrada em itens, removendo espaços em branco ao redor de cada item
    itens = [item.strip() for item in entrada.split(',')]
    
    # Imprime cada item com seu número correspondente
    for i, item in enumerate(itens, start=1):
        print(f"Item {i}: {item}")

# Exemplo de uso
if __name__ == "__main__":
    listar_compras()




**Exercício 4**
def celsius_para_fahrenheit():
    # Solicita ao usuário para digitar a temperatura em Celsius
    celsius = float(input("Digite a temperatura em graus Celsius: "))
    
    # Converte a temperatura para Fahrenheit
    fahrenheit = (celsius * 9/5) + 32
    
    # Imprime o resultado
    print(f"A temperatura em Fahrenheit é: {fahrenheit:.2f}")

# Exemplo de uso
if __name__ == "__main__":
    celsius_para_fahrenheit()





**Exercício 5**
def coletar_nomes():
    nomes = []
    
    while True:
        # Solicita ao usuário para digitar um nome
        nome = input("Digite um nome (ou 'sair' para encerrar): ")
        
        # Verifica se o usuário digitou 'sair'
        if nome.lower() == 'sair':
            break
        
        # Adiciona o nome à lista
        nomes.append(nome)
    
    # Imprime todos os nomes
    print("\nNomes digitados:")
    for i, nome in enumerate(nomes, start=1):
        print(f"Nome {i}: {nome}")

# Exemplo de uso
if __name__ == "__main__":
    coletar_nomes()
