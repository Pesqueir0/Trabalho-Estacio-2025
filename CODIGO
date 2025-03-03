def soma(a, b):
    return a + b

def subtracao(a, b):
    return a - b

def multiplicacao(a, b):
    return a * b

def divisao(a, b):
    if b == 0:
        return "Não é possível dividir por zero"
    else:
        return a / b

def calculadora(num1, num2, operacao):
    resultado = None

    if operacao == 'soma' or operacao == '+': 
        resultado = soma(num1, num2)
    elif operacao == 'subtracao' or operacao == '-': 
        resultado = subtracao(num1, num2)
    elif operacao == 'multiplicacao' or operacao == '*': 
        resultado = multiplicacao(num1, num2)
    elif operacao == 'divisao' or operacao == '/':  
        resultado = divisao(num1, num2)
    
    return resultado

while True:
    try:             
        numero_um = float(input("Digite o primeiro numero: "))        
        operacao = input("Insira a operação que deseja realizar (soma, subtração, multiplicacao ou divisao) " + 
                          "ou use os seus atalhos '+' , '-' , '*' ou '/' respectivamente: ")      
        if not (operacao == 'soma' or operacao == 'subtracao' or operacao == 'multiplicacao' 
                or operacao == 'divisao' or operacao in ['+', '-', '*', '/']):        
            raise ValueError("Operação invalida")  
                
        numero_dois = float(input("Digite o segundo numero: "))    
    except Exception as e:         
        print("Por favor digite um valor numérico valido!") 
        continue  
    
    resultado = calculadora(numero_um, numero_dois, operacao)      
    if isinstance(resultado, str):             
        print("Resultado: ", resultado)     
    else:                           
        print('Resultado da {} e {} usando {}: '.format(numero_um, numero_dois, operacao), resultado)  
    
    escolha = input("\nDeseja continuar? Digite 'N' ou 'n' para parar. Qualquer outra tecla rodará novamente: ")    
    if escolha == "N" or escolha == "n":
        break               
