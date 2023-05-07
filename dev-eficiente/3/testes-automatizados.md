# O papel dos testes automatizados no nosso código

## Qualidade

Testes automatizados são uma forma de garantir a qualidade do nosso código, mas não são a única forma. Um código não ter testes automatizados não necessariamente quer dizer que ele é de baixa qualidade.

Qual tipo de qualidade você entende que os testes trazem para o seu código?

- Confiabilidade na execução do código
  - Você testa o código por mais caminhos que o convencional.

Entretando, escrever testes não elimina a capacidade de escrever código e testes ruins.

## Testes de caixa branca

São considerados testes de caixa branca, ou white box, em inglês, aqueles em que a estrutura interna, código, design, intencionalidade e estratégias de desenvolvimento são conhecidas pelo testador e consideradas no ato do teste.

- Testes de cobertura: medem a extensão do código-fonte que foi executada durante o teste.
- Testes de fluxo de controle: avaliam o comportamento do software em diferentes caminhos de execução.
- Testes de integração: testam a interação entre diferentes módulos ou componentes do software.
- Testes de unidade: testam cada componente individualmente.

## Testes de caixa preta

Nos testes do tipo caixa preta, ou black box, em inglês, fatores como estrutura interna, código, design e estratégias de desenvolvimento são desconhecidos pelo testador.

Estes testes são conduzidos às cegas, e seu valor está justamente na oportunidade de observar como um usuário executa uma ação ou tarefa dentro da aplicação, ou com ela sem instruções, ou conhecimentos prévios.

- Testes de funcionalidade: verificam se o software realiza as funções especificadas no requisito.
- Testes de interface do usuário: verificam se a interface do usuário funciona corretamente.
- Testes de desempenho: medem o desempenho do software em termos de tempo de resposta e tempo de processamento.
- Testes de estresse: avaliam o comportamento do software em situações extremas, como alta carga de usuários ou sobrecarga de recursos.

## Quem programa escrevendo testes é mais lento?

Sim, necessariamente será mais lento, por você precisa escrever mais código. Porém você ganha em qualidade e confiabilidade.
Também é possível pensar que quanto maior a cobertura de testes mais complexo é a sua codebase, pois você precisa escrever mais testes (mais código) para cobrir todos os cenários. Logo tem mais esforço cognitivo e de manutenção, pois você precisa entender e manter os testes também.

## Estratégia

Temos um suposto ganho de qualidade ao desenvolver testes automatizados, e um aumento garantido de complexidade e esforço de manutenção. Como podemos então tirar o melhor proveito dos testes automatizados?

### O que eu vou testar no código?

- O código precisa ter 100% de cobertura de testes?

  - Não parece ruim, porém deve-se perguntar se o ganho de qualidade é proporcional a quantidade de esforço para escrever os testes. Se chegarmos em um nível onde o teste for gerado através de ferramentas automatizadas, seria menos custoso, e valeria mais a pena. Caso seja um esforço manual, é importante refletir sobre o custo benefício.

- Política de testes

  - Não pensar no teste como uma coisa que ajuda o programador, mas sim para maximizar a chance do código (programa) ser executado corretamente.
  - Deve-se pensar, onde é mais provável que o código tenha um erro? E focar os testes nesses pontos. Geralmente isso ocorre em laços, condicionais, e em pontos de integração com outros sistemas.

- O que eu vou testar no código?
  - 100% de cobertura em branchs de código e condicionais
