# sistema-financeiro-console
Projeto de estudo em Python

 faturamento = 1200
custo = 750.0

while True:
    print("\n--- MENU ---")
    print("1 - Adicionar faturamento")
    print("2 - Ver lucro")
    print("3 - Sair")

    opcao = input("Escolha uma opção: ")

    if opcao == "1":
        valor = float(input("Digite o valor a adicionar: "))
        faturamento += valor
        print("Faturamento atualizado!")

    elif opcao == "2":
        imposto = faturamento * 0.1
        lucro = faturamento - custo - imposto
        margem_lucro = lucro / faturamento

        print(f"Faturamento: R${faturamento}")
        print(f"Lucro: R${lucro}")
        print(f"Margem: {round(margem_lucro, 3)}")

    elif opcao == "3":
        print("Saindo...")
        break

    else:
        print("Opção inválida!")
