#definindo a palavra que vai ser colocada no jogo da forca
word = "elefante"

final = []
for i in range(len(word)):
    final.append('_')
erro = 5
soma = 0
acerto  = 0
erradas = []
print("Adivinhe a palavra abaixo:")

print("\n")
for i in range(len(final)):
    print(str(final[i]), end =' ')
while True:
    print("\n\nChances restantes:",erro,"\n")
    print("Letras erradas:")
    for i in range(len(erradas)):
        print(str(erradas[i]), end = '')
        
    if '_' not in final:
        acerto = 1
        break
    if erro == 0:
        break
    x = input("\nescolha uma letra: ")
    if x in final:
        print("erro, essa letra já foi escolhida antes!")
    
    else:
        for j in range (len(word)):
            if word[j] == x:
                final[j] = x
            
            else:
                if j == len(word) - 1 and x not in final:
                    erro = erro - 1
                    erradas.append(x)
                    print("\nletra errada")
                
    for i in range(0, len(final)):
        print(str(final[i]), end = ' ')
        
    print("\n")

if acerto == 1:
    print("\n\nParabés!! Você coseguiu. A palavra era", word)
else:
    print("\n\nVocê morreu")
