import random
import string

def gerar_codigo(codigos_gerados):
    letras_numeros = string.ascii_letters + string.digits

    while True:
        # Gerar os primeiros 24 caracteres
        parte1 = ''.join(random.choices(letras_numeros, k=24))
        # Gerar os próximos 26 caracteres após um ponto final
        parte2 = ''.join(random.choices(letras_numeros, k=26))
        codigo = f"{parte1}.{parte2}"

        if codigo not in codigos_gerados:
            return codigo

def gerar_codigos(quantidade):
    codigos_gerados = set()
    while len(codigos_gerados) < quantidade:
        codigos_gerados.add(gerar_codigo(codigos_gerados))
    return codigos_gerados

print("bem vindo ao: (welcome to:)")
print("--------------------------------------------------------------")
print("░██░░███░")
print("░█░█░█░░░")
print("░██░░███░")
print("░█████░░███░░█░██░████░██░░░█░░░░░████░░████░██░░░█░")
print("░░░█░░░█░░░█░█░█░░█░░░░█░█░░█░░░░█░░░░░░█░░░░█░█░░█░")
print("░░░█░░░█░░░█░██░░░███░░█░░█░█░░░░█░░██░░███░░█░░█░█░")
print("░░░█░░░█░░░█░█░█░░█░░░░█░░█░█░░░░█░░░█░░█░░░░█░░█░█░")
print("░░░█░░░░███░░█░██░████░█░░░██░░░░░███░░░████░█░░░██░")
print("by sr.raposo on viniciusrinaldi")
print("--------------------------------------------------------------")

print("How many tokens do you want to generate?")
quantidade = input("Quantos tokens você gostaria de gerar? ")

# Verifica se a entrada contém apenas números
while not quantidade.isdigit():
    print("Por favor, insira apenas números.")
    quantidade = input("Quantos tokens você gostaria de gerar? ")

quantidade = int(quantidade)
codigos_gerados = gerar_codigos(quantidade)

for codigo in codigos_gerados:
    print(codigo)
    
if quantidade == 1:
    print(quantidade, "token foi gerado com sucesso!")
else:
    print(quantidade, "tokens foram gerados com sucesso!")
