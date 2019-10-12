# simulador-consultoria
Código capaz de simular o lucro gerado a partir da quantia investida, taxa de aumento das ações e prazo pré estabelecido pelo usuário. Futuramente acoplado com aplicativos e sistemas de consultoria financeira.

CI =  int(input('Insira seu Capital Inicial!(em reais)'))
INVESTIMENTO =  int(input('Insira o valor que deseja investir(em reais)'))
PRAZO =  int(input('Insira o Prazo que pretende ter resultados (em meses)'))
TAXA = float(input('Insira uma taxa de váriação de rendimento (sendo a taxa > 1)'))
print('Seu rendimento de acordo com o seu prazo e ataxa de crescimento será de:')
print(((INVESTIMENTO*PRAZO)*TAXA)-(INVESTIMENTO*PRAZO))
if CI/3 > INVESTIMENTO:
    print('Seu Investimento não será tão arriscado, procure informações de como investir na Trilha 2')
if CI%PRAZO > 0:
        print('Você terá um pouco de retorno a curto prazo, para mais informações procure a Trilha 3')
if CI/3 < INVESTIMENTO:
    print('Seu Investimento possui um certo risco de acordo com outras situações, para mais informações procure a Trilha 2')
    if INVESTIMENTO >= CI:
        print('Você não está indo por um bom caminho, para mais informações de como investir procure a Trilha 3')
if CI%PRAZO == 0:
    print('Seu investimento não terá grande rendimento, para mudar está situação melhore seu jeito de Investir com as dicas da trilha 4')
