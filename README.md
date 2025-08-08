# imc4
print("Bem-vindo à Calculadora de IMC!\n")

nome = input("Qual é o seu nome? ")
print(f"Olá, {nome}!")

idade = input("Qual sua idade? ")
peso = float(input("Qual seu peso? (em KG) "))
altura = float(input("Qual sua altura em metros? (use ponto) "))

print("\nCalculando seu IMC...\n")

imc = peso / (altura ** 2)


print(f"{nome}, seu IMC é: {imc:.2f}\n")

if imc < 16:
    print("⚠️ Magreza grave — procure um médico ou nutricionista.")
elif imc < 17:
    print("‼️ Magreza moderada — reveja sua alimentação.")
elif imc < 18.5:
    print("❗ Magreza leve — atenção à sua saúde.")
elif imc < 25:
    print("🔱Saudável — parabéns!")
elif imc < 30:
    print("❕ Sobrepeso — atenção à sua alimentação.")
elif imc < 35:
    print("❗Obesidade Grau I — consulte um profissional de saúde.")
elif imc < 40:
    print("‼️Obesidade Grau II (severa) — acompanhamento médico recomendado.")
else:
    print("⚠️ Obesidade Grau III (mórbida) — risco alto, procure ajuda especializada.")
