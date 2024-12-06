#desafio estruturas condicionais reajuste de salario 
salario_atual = float (input('salario atual é : R$'))

if salario_atual <=280.00:
  percentual_aumento = 20
elif salario_atual <=700.00:
  percentual_aumento = 15
elif salario_atual <=1500.00:
  percentual_aumento = 10
else: 
  percentual_aumento = 5
print(percentual_aumento)

valor_aumento = salario_atual * percentual_aumento / 100
print(valor_aumento)
novo_salario = salario_atual + valor_aumento
print(novo_salario)

inflação = 3.8
valor_aumento_real = valor_aumento - (salario_atual * inflação / 100)
print(valor_aumento_real)

print ('resultado do reajuste')
print ('salario antes do reauste: R$ {salario_atual}')
print ('percentual de aumento aplicado: {percentual_aumento}%')
print ('valor do aumento: R$ {valor_aumento}')
print ('novo salario: R$ {novo_salario}')
print ( 'valor do aumento real (descontado a inflação):R$ {valor_aumento_real}')
