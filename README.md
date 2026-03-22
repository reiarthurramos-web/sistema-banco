# sistema financeiro simples
Projeto de estudo em Python que simula um sistema financeiro simples com menu interativo.


faturamento = 1200
custo = 750.0

while True:
    print("\n--- MENU ---")
    print("1 - Adicionar faturamento")
    print("2 - Ver lucro")
    print("3 - Ver custo")
    print("4 - Sair")

    opcao = input("Escolha uma opção: ")

    if opcao == "1":
        valor = float(input("Digite o valor a adicionar: R$"))
        faturamento += valor
        print("Faturamento atualizado!")

    elif opcao == "2":
        imposto = faturamento * 0.1
        lucro = faturamento - custo - imposto
        margem_lucro = lucro / faturamento

        print(f"\nFaturamento: R${faturamento}")
        print(f"Lucro: R${lucro}")
        print(f"Margem de lucro: {round(margem_lucro, 3)}")

    elif opcao == "3":
        print(f"\nCusto atual: R${custo}")

    elif opcao == "4":
        print("Saindo do sistema...")
        break

    else:
        print("Opção inválida, tente novamente!")




## Funcionalidades
- Adicionar faturamento
- Visualizar lucro
- Visualizar custo
- Calcular margem de lucro
- Menu interativo no console

## Tecnologias
- Python

## Como executar
1. Instale o Python no seu computador
2. Baixe o arquivo do projeto
3. Execute no terminal:

python nome_do_arquivo.py

## Objetivo
Este projeto foi desenvolvido para praticar lógica de programação, uso de loops (while), condicionais (if/else) e entrada de dados com input.

## Autor
Arthur (estudante de programação)
