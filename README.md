from dnd_calculo_vd.funçao_dnd_calculo_vd import dnd_calculo_vd
nome = input("qual o nome do seu personagem?\n")
clases = int(input("quantas classes vc tem?\n"))
ldados_de_vida = []
lniveis = []
for i in range(clases):
    dados_de_vida = int(input(f"qual seu dado de vida da sua {i+1}º classe? \n"))
    niveis = int(input(f'qual seu nivel(s) na sua {i+1}º classe? \n'))
    ldados_de_vida.append(dados_de_vida)
    lniveis.append(niveis)
constituiçao = int(input('qual seu modificador de constituição\n'))
print(f"{nome} tem {dnd_calculo_vd(ldados_de_vida , lniveis , constituiçao)} pontos de vida" )
