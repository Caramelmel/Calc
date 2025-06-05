import math

def soma(a, b):
    return a + b
def subtracao(a, b):
    return a - b
def multiplicacao(a, b):
    return a * b
def divisao(a, b):
    if b == 0:
        return "Erro: Divisão por zero!"
    return a / b
def potencia(a, b):
    return a ** b
def raiz_quadrada(a):
    if a < 0:
        return "Erro: Raiz quadrada de número negativo!"
    return math.sqrt(a)
def exibir_menu():
    print("\n--- Calculadora ---")
    print("1. Soma")
    print("2. Subtração")
    print("3. Multiplicação")
    print("4. Divisão")
    print("5. Potência")
    print("6. Raiz Quadrada")
    print("0. Sair")
def main():
    while True:
        exibir_menu()
        try:
            opcao = int(input("Escolha uma opção: "))
            if opcao == 0:
                print("Saindo da calculadora. Até mais!")
                break
            if opcao == 6:
                numero = float(input("Digite o número: "))
                resultado = raiz_quadrada(numero)
            elif 1 <= opcao <= 5:
                numero1 = float(input("Digite o primeiro número: "))
                numero2 = float(input("Digite o segundo número: "))
                if opcao == 1:
                    resultado = soma(numero1, numero2)
                elif opcao == 2:
                    resultado = subtracao(numero1, numero2)
                elif opcao == 3:
                    resultado = multiplicacao(numero1, numero2)
                elif opcao == 4:
                    resultado = divisao(numero1, numero2)
                elif opcao == 5:
                    resultado = potencia(numero1, numero2)
            else:
                print("Opção inválida! Tente novamente.")
                continue
            print(f"O resultado da operação é: {resultado}")
        except ValueError:
            print("Erro: Por favor, digite números válidos.")
        except Exception as e:
            print(f"Erro inesperado: {e}")
