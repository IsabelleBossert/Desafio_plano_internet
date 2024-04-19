print('\033[1;37mTabela de Planos'.center(20, ' '))
print('''
\033[1;35mPlano Essencial Fibra - 50Mbps | \n
Plano Prata Fibra - 100Mbps    | \n
Plano Premium Fibra - 300Mbps  |

''')
consumo = float(input('\033[1;37mQual a média de consumo mensal em GB?'))

def recomendar_plano(consumo):
    if consumo <= 10:
        print('Sugerimos o Plano Essencial Fibra - 50mbps, recomendado para consumo até 10GB. ')

    elif consumo > 10 and consumo <= 20:
        print('Sugerimos o Plano Prata Fibra - 100Mbps, recomendado para consumo até 20GB. ')

    elif consumo > 20:
        print('Sugerimos o Plano Premium Fibra - 100Mbps, recomendado para consumo acima de 20GB.')

    else:
        print('Opcao inválida!')


recomendar_plano(consumo)
