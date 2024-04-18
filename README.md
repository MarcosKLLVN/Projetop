import random

saldo = 1000
valor_aposta = 0
resultado = ""

print ("Bem-vindo ao jogo do tigrinho")

while saldo > 0:
    print (f"Saldo dispoível: $ {saldo}")
    valor_aposta = int(input("Digite o valor de aposta: "))
                       
    if valor_aposta > saldo:
        print ("Você não possui saldo suficiente para fazer esta aposta.")
        
    else: valor_aposta < saldo 
    print("Aguarde")
    
    saldo -= valor_aposta
    print (f"Aposta realizada. Saldo. Saldo restante: ${saldo}")
    
    print("Jogo em andammento 3")
    print("Jogo em andammento 2")
    print("Jogo em andammento 1")

    resultado = random.choice (["vitória", "derrota"])
    
    if resultado == "vitória":
        print("Parabéns!! Você ganhou a aposta.")
        saldo += valor_aposta * 2
    else: 
        print("Que pena! Você perdeu a aposta.")
        
print("Seu saldo acabou. O jogo acabou.")
