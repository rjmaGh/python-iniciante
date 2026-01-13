from time import sleep
def finalizando_compra():
    print('-' *100)
    final = int(input('''            Deseja finalizar a compra? 
    [{}1{}] Efetuar pagamento         [{}2{}] Cancelar compra
    Opção: ''' .format('\033[32;1m', '\033[m', '\033[1;31m' ,'\033[m' )))
    sleep(1)
    if final == 1:
        print()
        print('    EFETUANDO COMPRA...')
        sleep(2)
        print()
        print('\033[32;1m         COMPRA FINALIZADA COM SUCESSO.')
        print('\033[32;1m-\033[m' *100)
    elif final ==2:
        print()
        print('          \033[31;1mCOMPRA CANCELADA.')
        print('\033[1;31m-\033[m' *100)
    else:
        print('\033[31mOpção INVÁLIDA. TENTE NOVAMENTE.')
    sleep(1)
    print('\033[30;1mMuito obrigado pela sua visita, esperamos que volte sempre :)'.upper())

#FUNCIONALIDADE - DEF - Procedimento -, CRIADA PARA SER COLOCADA DENTRO DO NOSSO PROGRAMA QUANDO NECESSÁRIO.
# -------------- INICIO DO PROGRAMA ---------------
print('\033[1;32m-'*23, '\033[m')
print('{} LOJAS KIRAandLUCKY   {}|' .format('\033[1;34m', '\033[38m'))
print('\033[33m-'*23, '\033[m')
sleep(1)
compras = float(input('Valor total da(s) compra(s): R$'))
print()
print('       Temos algumas condições dependendo da sua forma de pagamento..')
print('-'*100)

print('''              Selecione a forma que deseja prosseguir:
[{}1{}] À vista (5 à 10% desc) [{}2{}] Até 2x no cartão (SEM desc) [{}3{}] 3 à 6x no cartão (20% de {}JUROS{})'''
      .format('\033[32;1m', '\033[m', '\033[32;1m','\033[m', '\033[32;1m','\033[m', '\033[31;1m','\033[m'))
fp = int(input('Opção: '))
print('-'*100)
sleep(1)

if fp == 1:
    print('''         Para pagamento à vista, temos duas opções:
[{}1{}] Dinheiro/cheque (10% de desc)   [{}2{}] Cartão (5% de desc)''' .format('\033[32;1m',  '\033[m' , '\033[32;1m', '\033[m'))
    pagamento = int(input('Qual deseja? '))
    sleep(1)
    if pagamento == 1:
        desconto = compras * 10 /100
        novovalor = compras - desconto
        print('\033[1mCom o desconto de R${:.2f}, suas compras sairão pelo valor de R${:.2f}\033[m' .format(desconto, novovalor))
        sleep(2)
        finalizando_compra()

    elif pagamento == 2:
        desconto = compras *5 /100
        novovalor = compras - desconto
        print('\033[1mCom o desconto de R${:.2f}, suas compras sairão pelo valor de R${:.2f}\033[m'.format(desconto, novovalor))
        sleep(2)
        finalizando_compra()
    else:
        print('\033[31mOpção inválida. TENTE NOVAMENTE.')

elif fp == 2:
    parcela = compras / 2
    print('{}Suas compras em até 2x no cartão, sairão pelo valor normal, de R${:.2f}{} '.format('\033[1m', compras, '\033[1m'))
    sleep(1)
    print('{}O valor das parcelas será de R${:.2f}{}' .format('\033[1m', parcela, '\033[m'))
    sleep(2)
    finalizando_compra()

elif fp == 3:
    valorjuros = (compras * 20) /100 + compras
    print('''\033[1mCom os juros, o valor final das compras, será de R${:.2f}
                    Em quantas vezes deseja parcelar?''' .format(valorjuros))
    sleep(2)
    print('[{}3{}] 3x no cartão [{}4{}] 4x no cartão [{}5{}] 5x no cartão [{}6{}] 6x no cartão' .format('\033[1;32m', '\033[m', '\033[1;32m',
    '\033[m', '\033[1;32m', '\033[m', '\033[1;32m', '\033[m'))
    pagamento = int(input('Opção: '))
    parcela = valorjuros / pagamento
    sleep(2)
    print('\033[1mPagando em {}x no cartão, suas parcelas serão de R${:.2f} por mês.' .format(pagamento, parcela))
    sleep(2)
    finalizando_compra()

else:
    print('\033[31mOpção inválida. TENTE NOVAMENTE')


