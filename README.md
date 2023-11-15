try:
    numero_1 = input("Digite um número: ")
    operador = input("Informe o operador da conta que deseja realizar: ")
    numero_2 = input("Digite outro número: ")

    numero_format_1 = int(numero_1) or float(numero_1)
    numero_format_2 = int(numero_2) or float(numero_2)

    soma = numero_format_1 + numero_format_2
    subtracao = numero_format_1 - numero_format_2
    multiplicacao = numero_format_1 * numero_format_2
    divisao = numero_format_1 / numero_format_2

    try:
        if operador == '+':
            print(f'{numero_format_1} + {numero_format_2} = {soma}')
        elif operador == '-':
            print(f'{numero_format_1} - {numero_format_2} = {subtracao}')
        elif operador == '*':
            print(f'{numero_format_1} * {numero_format_2} = {multiplicacao}')
        elif operador == '-':
            print(f'{numero_format_1} / {numero_format_2} = {divisao}')
    except:
        print("Informe somente operadores validos.")
except:
    print("Informe somente números.")
