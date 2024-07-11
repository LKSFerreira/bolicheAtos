# Jogo de Boliche: Calculadora de Pontuação

Este projeto implementa um algoritmo para calcular a pontuação de um jogo de boliche, além de explorar a tecnologia de embedding para integração e execução de código em uma plataforma externa.

## Descrição do Algoritmo

O jogo de boliche consiste em 10 frames, onde cada frame pode resultar em um strike, spare ou open frame:

- **Strike:** Derruba todos os 10 pinos no primeiro arremesso. Pontuação = 10 + número de pinos derrubados nos próximos 2 arremessos.
- **Spare:** Derruba todos os 10 pinos com dois arremessos. Pontuação = 10 + número de pinos derrubados no próximo arremesso.
- **Open Frame:** Derruba menos de 10 pinos em dois arremessos. Pontuação = número de pinos derrubados.

No décimo frame, há regras especiais para strikes e spares, onde bolas extras podem ser concedidas.

## Funcionalidades Implementadas

- **arremesso(pinos: int)**: Registra o número de pinos derrubados em cada arremesso.
- **pontuação() -> int**: Calcula e retorna a pontuação total do jogo ao final.

### Exemplos de Pontuação

Exemplo de uma partida de boliche com três frames:

1. Frame 1 → X (strike)
2. Frame 2 → 5/ (spare)
3. Frame 3 → 9 0 (open frame)

Pontuação:
- Frame 1: 10 (strike) + 5 (arremesso 1 do Frame 2) + 5 (arremesso 2 do Frame 2) = 20
- Frame 2: 5 (arremesso 1 do Frame 2) + 5 (arremesso 2 do Frame 2) + 9 (arremesso 1 do Frame 3) = 19
- Frame 3: 9 + 0 = 9

Pontuação total: 20 + 19 + 9 = 48

### Demonstração de Embedding

Este projeto utiliza a plataforma Trinket.io para demonstrar a execução de código Python incorporado em uma página web. O exemplo prático é a integração do jogo de boliche com a plataforma de embedding, mostrando como diferentes tecnologias podem ser integradas para oferecer uma experiência interativa.

## Riscos e Considerações

Embora o embedding de código externo ofereça flexibilidade e funcionalidades avançadas, há alguns pontos de atenção a serem considerados:

- **Segurança:** Incorporar código de terceiros pode introduzir vulnerabilidades de segurança se não forem tomadas precauções adequadas.
  
- **Dependência Externa:** Dependendo da plataforma de embedding, pode haver limitações de desempenho, estabilidade ou disponibilidade que afetam a experiência do usuário final.
  
- **Compatibilidade:** Garantir que o código incorporado funcione corretamente em diferentes navegadores e dispositivos pode ser um desafio técnico.

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para forkar este projeto, fazer melhorias e enviar um pull request.
