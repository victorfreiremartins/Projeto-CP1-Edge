# Projeto-CP1-Edge

# RM dos alunos envolvidos no projeto.
Bruno Biletsky - RM: 554739
Eduardo Vicentini Levy - RM: 554561
Enrico Ricarte Rodrigues - RM: 558571
Victor Freire - RM: 556191
Matheus Gushi - RM: 556935

# Projeto Sensor de Luminosidade

O projeto nasceu da necessidade de monitorar a luminosidade, uma vez que ela desempenha um papel crucial na preservação da qualidade do vinho. A exposição inadequada à luz pode afetar negativamente o sabor e a durabilidade do vinho, tornando essencial o controle preciso da luminosidade durante o armazenamento e o processo de envelhecimento. Este projeto oferece uma solução automatizada para monitorar a luminosidade do ambiente e fornecer alertas visuais e sonoros quando os níveis ultrapassam os limites desejados, garantindo assim a integridade do produto final.

## Funcionalidades

- O sensor LDR (Light Dependent Resistor) é utilizado para detectar a intensidade de luz no ambiente. No contexto do Arduino, ele pode ser utilizado em projetos que requerem controle de luminosidade, como acionamento automático de luzes, detecção de presença, entre outros.

- O sistema implementará um feedback visual e sonoro com base na luminosidade detectada pelo sensor LDR. Quando a luminosidade atingir um nível alto, o buzzer emitirá um sinal sonoro e um LED vermelho será acionado. Em condições de luminosidade média, um LED amarelo será ativado. Em baixa luminosidade, um LED verde será acionado.

## Instalação

Para configurar a sensibilidade do sensor, é necessário reconfigurar a função "map" do código para se adequar ao controle de luminosidade necessário. Além disso, será necessário possuir um sensor LDR, três LEDs (verde, amarelo, vermelho), três resistores (um para cada LED) e um resistor 10kΩ para o LDR.

Instruções detalhadas sobre a configuração física dos componentes e a integração com o código podem ser encontradas na simulação do tinkercad.

## Uso

Além disso, o projeto pode ser utilizado em qualquer necessidade de monitorar e representar a situação atual da luminosidade. Seja para controlar a luz em um ambiente de exposição de obras de arte sensíveis à luz, monitorar a luminosidade em uma estufa para plantas delicadas, ou qualquer outra aplicação que exija um controle preciso da luminosidade, este sistema oferece uma solução versátil e adaptável.

## Créditos

Agradecimentos ao professor Fábio Cabrini pelo apoio e orientação no desenvolvimento deste projeto. Também gostaríamos de agradecer aos alunos e companheiros de projeto Bruno Biletsky, Victor Freire, Enrico Ricarte e Eduardo Levy pela colaboração e dedicação.
