# textjogoadv
#jogo de adivinhação
from random import randint
pc = randint(1, 10)
jogador = int(input('vamos jogar um game, digite de 1 a 10: '))
vencedor = 0
tentativas = 0
while not vencedor == 1:
    if pc == jogador:
        print(f'vc venceu com {tentativas} tentativas!!')
        vencedor += 1
    else:
        tentativas += 1
        if jogador < pc:
            jogador = int(input('Quase tente um pouco mais...!!!: '))
        else:
            jogador = int(input('Quase tente um pouco menos...!!!: '))