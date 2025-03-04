# Qualidade de Software BDD


### Explicação do Gherkin
O Gherkin é uma linguagem simples e estruturada usada para descrever o comportamento esperado de um software em termos de cenários de uso. Ele é fácil de entender, mesmo para pessoas não técnicas, e serve como uma documentação viva do software. Com o Gherkin, equipes podem colaborar na especificação de requisitos e na automação de testes para garantir que o software atenda às necessidades dos usuários finais.

### Gherkin

Feature: Sistema de Locação de Carros

  Scenario: Reserva antecipada de um carro de luxo com desconto
    Given um cliente deseja alugar um carro de luxo
    And o cliente realiza a reserva com antecedência de pelo menos uma semana
    When o cliente completa a reserva
    Then o sistema deve oferecer um desconto especial no valor total da locação

  Scenario: Locação de última hora de um carro utilitário
    Given um cliente necessita alugar um carro utilitário de última hora
    And o cliente não possui uma reserva prévia
    When o cliente solicita a locação
    Then o sistema deve encontrar um veículo disponível
    And o sistema deve processar a locação rapidamente
    And o sistema deve aplicar um custo adicional devido à demanda urgente
