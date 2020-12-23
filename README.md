# DESAFIO de ROBÓTICA - 2021

![banner](https://github.com/MatheusFranca-dev/desafiorobotica/blob/master/resources/banner.png)

Este repositório contém os arquivos necessários para a realização da simulação do **DESAFIO** referente ao **Laboratório de Robótica e Sistemas Autônomos** para atuação como estagiário de graduação no **SENAI CIMATEC**.

# Organização

A organização das pastas é a seguinte:

- `resources` - Arquivos de suporte geral.

- `webots_content` - Contém o **mundo** e o **controle** para a simulação do desafio. Você pode carregá-los dentro do simulador Webots.

# Desenvolvimento

![banner](https://github.com/MatheusFranca-dev/desafiorobotica/blob/master/resources/desafio-fast.gif)

O código do desafio pode ser encontrado em desafio.c(). O trajeto foi realizado em 1 minuto e 11 segundo ao todo. 
A explicação pode ser vista a seguir: 

**1.** Para o robô parar no local indicado foi adicionado um lightsensor() no seu extensioSlot(). Vale ressaltar que além dos próprios sensores, foi utilizado apenas o lightsensor a mais.    

**2.** Foi definido um valor máximo para o sensor de luz, que indica quando ele deve parar. 

**3.** Os sensores então foram inicializados, e os pesos que cada sensor tem em relação a movimentação do robô selecionados.

**4.** Na loop da simulação foi então lidos os seus valores e o robô foi iniciado para frente. 

**5.** Então, se a leitura do sensor de luz for maior ou igual ao valor definido, o robô para (chegamos na luminaria).

**6.** Se ainda não chegou no objetivo, avalie os pesos dos sensores e desvie dos obstaculoes e vá para frente. 

**7.** Os passos 5 e 6 armazenam as velocidades escolhidas em um vetor, para que só depois seja atribuido ao par de motores. 


**Sem esforço não há recompensa!**

'This is the way.'
