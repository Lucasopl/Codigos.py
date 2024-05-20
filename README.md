#feito para dar um aumento para um colaborador e ja fazer o calculo menos o os 8% de descontos
def calcular_salario_final(salario):
    aumento = salario * 0.15
    salario_com_aumento = salario + aumento
    desconto_imposto = salario_com_aumento * 0.08
    salario_final = salario_com_aumento - desconto_imposto
    return salario_com_aumento, salario_final

def main():
    salario = float(input("Digite o salário do funcionário: "))
    salario_com_aumento, salario_final = calcular_salario_final(salario)
    print(f"Salário inicial: R${salario:.2f}")
    print(f"Salário com aumento: R${salario_com_aumento:.2f}")
    print(f"Salário final após desconto de impostos: R${salario_final:.2f}")

if __name__ == "__main__":
    main()
