# Relatório de Progresso I [12/05 - 18/05]

Simulação de agentes com NetLogo: **Agricultura inteligente com agentes**

O objetivo deste projeto é modelar e simular um sistema agrícola inteligente que utiliza sensores e irrigadores para monitorar e manter a umidade ideal do solo, com influência de fatores climáticos como chuva, pragas e eventos externos. A simulação busca representar de forma visual e lógica o comportamento do solo e das plantas em diferentes condições, auxiliando no estudo de sistemas multiagentes e simulações ambientais.

## Agentes implementados até o momento

### `Plantas`
- Representam cultivos no solo.
- Mudam de estado (saudável, desidratada, murcha, morta) com base na umidade do solo em que estão plantadas.

### `Sensores`
- Monitoram a umidade do solo ao redor de sua posição em um raio de 1,5 (patches).
- Imprimem no console os níveis de umidade das plantas monitoradas.

### `Irrigadores`
- Responsáveis por irrigar as plantas monitoradas pelos sensores em um raio de 2,0.
- Ativam a irrigação quando o sensor detecta a umidade do solo abaixo de 60%.

### `Chuvas`
- Evento climático aleatório com duração limitada.
- Gotas se movem no ambiente e aumentam a umidade dos patches onde caem.
- A chuva interfere no funcionamento do irrigador, que pausa a irrigação durante o evento.


## Já implementado

- Inicialização do ambiente com patches representando solo e variação de cor conforme umidade.
- Experimento com 3 plantas, sendo 2 monitoradas pelo sensor e 1 não monitorada.
- Sistema de evaporação da umidade do solo.
- Monitoramento de umidade em tempo real pelos sensores.
- Irrigação automatizada por irrigadores conforme necessidade.
- Evento climático de chuva com comportamento visual (animação de gotas).
- Atualização visual dos estados das plantas.


## O que ainda será feito

- [ ] Adicionar novos tipos de agente: pragas ou doenças que afetem as plantas, e um agricultor que fará intervenção manual em plantas não monitoradas.
- [ ] Registrar dados estatísticos em componentes de monitores (ex: quantidade de irrigação, número de plantas mortas/salvas, variação do solo).
- [ ] Para a realização de mais testes, adicionar componentes de interface para controle da chance de chuva, porcentagem de evaporação do solo, etc.
- [ ] Evento de inundação das plantas devido a chuvas intensas, o que precisará de intervenção humana e também será monitorado pelos agentes de sensores.
- [ ] Criar um gráfico em tempo real com variação de umidade média do solo onde as plantas estão.

## Conclusão do progesso

Até o momento o modelo cumpre o papel de representar um sistema básico de agricultura inteligente com múltiplos agentes. Baseado em programar procedimentos, o uso do NetLogo tem permitido testar conceitos de simulação multiagente de maneira acessível e visual. Com a evolução do projeto, deve ser permitido observar interações mais complexas entre agentes e eventos, contribuindo para o entendimento de sistemas autônomos no contexto agrícola.