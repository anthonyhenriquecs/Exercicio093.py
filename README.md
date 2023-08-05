# Exercicio093.py

jogador = dict()
partidas = []
jogador['nome'] = str(input('NOME DO JOGADOR:'))
tot = int(input(f'Quantas partidas {jogador["nome"]} jogou?'))
for c in range(0, tot):
    partidas.append(int(input(f'Quantos gols na partida {c+1}? ')))
jogador['gols'] = partidas[:]
jogador['soma'] = sum(partidas)
print('=-'*30)
print(jogador)
print('=-'*30)
for k, v in jogador.items():
    print(f'O campo {k}, tem o valor {v}')
print('=-' * 30)
print(f'O jogador {jogador["nome"]} jogou {len(jogador["gols"])} partidas')
for i, v in enumerate(jogador['gols']):
    print(f'Na partida {i+1} fez {v} gols ')
print(f'Com um total de {jogador["soma"]} gols' )
