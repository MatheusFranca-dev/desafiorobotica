# DESAFIO de ROBÓTICA - 2021

![banner](https://github.com/MatheusFranca-dev/desafiorobotica/blob/master/resources/banner.png)

Este repositório contém os arquivos necessários para a realização da simulação do **DESAFIO** referente ao **Laboratório de Robótica e Sistemas Autônomos** para atuação como estagiário de graduação no **SENAI CIMATEC**.

# Organização

A organização das pastas é a seguinte:

- `resources` - Arquivos de suporte geral.

- `webots_content` - Contém o **mundo** e o **controle** para a simulação do desafio. Você pode carregá-los dentro do simulador Webots. 

# Desenvolvimento

![banner](https://github.com/MatheusFranca-dev/desafiorobotica/blob/master/resources/desafio-fast.gif)

O código e o vídeo do desafio podem ser encontrados respectivamente em: [desafio.c](https://github.com/MatheusFranca-dev/desafiorobotica/blob/master/webots_content/controllers/desafio/desafio.c) e [desafio.mkv](https://github.com/MatheusFranca-dev/desafiorobotica/blob/master/resources/desafio.mkv). O trajeto foi realizado em 1 minuto e 11 segundos ao todo. 
A explicação pode ser vista a seguir: 

**1.** Para o robô parar no local indicado foi adicionado um [lightsensor](https://www.cyberbotics.com/doc/reference/lightsensor) no seu extensionSlot. Vale ressaltar que além dos próprios sensores, foi utilizado apenas o lightsensor a mais.   

**2.** Foi definido um valor máximo para o sensor de luz, que indica quando ele deve parar.

**3.** Os sensores foram inicializados, e os pesos que cada sensor tem em relação a movimentação do robô foram selecionados.

**4.** No loop da simulação foram então lidos os seus valores e o robô foi iniciado se movimentando para frente.

**5.** Então, se a leitura do sensor de luz for maior ou igual ao valor definido, o robô para (chegamos na luminária).

**6.** Se ainda não chegou no objetivo, avalie os pesos dos sensores, desvie dos obstáculos e vá para frente.

**7.** Os passos 5 e 6 armazenam as velocidades escolhidas em um vetor, para que só depois seja atribuído ao par de motores.


**Sem esforço não há recompensa!**

'This is the way.'
