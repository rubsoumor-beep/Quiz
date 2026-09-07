import sys
from time import sleep
from playsound3 import playsound

def main():
 while True:
  sys.stdout.reconfigure(line_buffering=True)
  print("Adivinhe o jogo pelo toque")
  sleep(2)
  print("Esta pronto?")
  sleep(2)
  playsound('02-title_IjqoHXpW.mp3')
  print("Eai que jogo é esse sabe?")
  sleep(2)
  resposta1 = (int(input("1-Super Mario\n2-Street Fighter\n3-Super Metroid\n4-Mega Man X\n")))
  if resposta1 == 1:
   print("Voçê acertou(Super Mario)")
   playsound("47. Course Clear.mp3")
   print("Adivinhe o jogo pelo toque")
   sleep(2)
   playsound("02-house_jpmDUk1Z.mp3")
   resposta2 = (int(input("1-Ninja Turtles\n2-Zelda\n3-Contra III\n4-Aladdin\n")))
   if resposta2 == 2:
    print("Voçê acertou(Zelda)")
    playsound('09 Small Item Catch.mp3')
    sleep(2)
    print("Adivinhe o jogo pelo toque")
    sleep(2)
    playsound('02-theme_mG3unxkq.mp3')
    resposta3 = (int(input("1-Castlevania IV\n2-Secret of Mana\n3-Donkey Kong\n4-Power Rangers\n")))
    if resposta3 == 3:
     print("Voçê acertou(Donkey Kong)")
     playsound('50 - End of Stage.mp3')
     print("Adivinhe o jogo pelo toque")
     sleep(2)
     playsound('01. Title Screen.mp3')
     resposta4 = (int(input("1-Super Bomberman 3\n2-Magical Quest\n3-Killer Instinct:\n4-Sonic\n")))
     if resposta4 == 4:
         print("Voçê acertou(Sonic)")
         playsound('03-ocean-view_PgTXPoDN.mp3')
         print("Voçê venceu o quiz, obrigado por jogar ;D")
         sleep(5)
         playsound('03. Ground BGM (Hurry Up!).mp3')
     elif resposta4 != 4:
         print("Voçê errou a resposta")
         playsound('18. Game Over.mp3')
         print("Continuar?")
         sleep(2)
         cont = int(input("1 para Sim ou 2 para Não\n"))
         if cont == 1:
          print("")
         else:
          print("Fim de jogo")
          break
    elif resposta3 != 3:
     print("Voçê errou a resposta")
     playsound('110-game-over_uFE4VUjI.mp3')
     print("Continuar?")
     sleep(2)
     cont = int(input("1 para Sim ou 2 para Não\n"))
     if cont == 1:
        print("")
     else:
        print("Fim de jogo")
        break
   elif resposta2 != 2:
    print("Voçê errou a resposta")
    playsound('73 Game Over.mp3')
    print("Continuar?")
    sleep(2)
    cont = int(input("1 para Sim ou 2 para Não\n"))
    if cont == 1:
     print("")
    else:
     print("Fim de jogo")
     break
  elif resposta1 != 1:
   print("Voçê errou a resposta")
   playsound("52. Game Over.mp3")
   print("Continuar?")
   sleep(2)
   cont = int(input("1 para Sim ou 2 para Não\n"))
   if cont == 1:
    print("")
   else:
    print("Fim de jogo")
    break

if __name__ =="__main__":
     main()
