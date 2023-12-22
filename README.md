# Projeto3-Micro-Controladores Leituras analógicas e Display LCD
## Integrantes:
Diogo Barboza de Souza - NUSP: 12745657  
Yudi Asano Ramos - NUPS: 12873553  

# Desenvolvimento  
A leitura de sinais analógicos é crucial em sistemas embarcados, já que variáveis do mundo real, como temperatura e pressão, não são discretizadas. Para essa conversão, os conversores A/D são essenciais, e o uso de microcontroladores com módulos ADC internos simplifica esse processo. No caso do PIC18F4550, seu módulo ADC é configurável por registradores, facilitando sua integração com a linguagem C pelo compilador MikroC PRO for PIC, que oferece bibliotecas otimizadas para essa tarefa, o que foi usado nesse projeto.  

Visto isso, o PIC18F4550 foi programado para realizar a conversão ADC e exibir os resultados em um display LCD. Utilizando o material dado, datasheet e o manual do Kit EasyPICv7, e configurados os módulos ADC e LCD no microcontrolador.   

O circuito em questão feito para o codigo:  
![image](https://github.com/Yudiaramos/Projeto3-Micro-Controladores/assets/113189511/0ba043d4-a9af-4daa-bb53-c55001ad1bb9)  
Foi usado a frequência do clock de 8 MHz, o display está em sua configuração de 4 bits, isto é, D4-D7 para a escrita, enquanto D0-D3 estão conectados ao GND. Além de que as entradas analógicas são dadas pela porta A5, onde são ofertadas os sinais analogicos.

# Resultados
Os resultados são visíveis no display LCD, onde primeiramente é necessario as entradas analógicas, como a leitura de um potenciômetro, que é convertida pelo módulo ADC. O código realiza essa conversão e, em seguida, o LCD é responsável por exibir os resultados da conversão analógico-digital. Essa abordagem permite uma interface clara e compreensível para representar valores analógicos de forma digitalizada no display.
