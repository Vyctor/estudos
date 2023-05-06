# Sumário

## 1

## 2

## 3 - Qualidade de código e software em aplicações modernas

- [Pattern 2: Services 100% coesos](./dev-eficiente/)

- Números de linhas isoladamente não indica a complexidade de um arquivo. Devemos sempre observar a coesão do arquivo, ou seja, se ele está fazendo apenas uma coisa, aplicando a teoria da complexidade cognitiva que diz que o cérebro humano consegue processar apenas 7 itens de uma vez. Se um arquivo possui mais de 7 responsabilidades, ele é considerado complexo.
- Um arquivo com mais de 7 responsabilidades é considerado complexo e deve ser refatorado.
- Uma classe que não é nem um application service, nem um controller ou entidade e não tem uma especialização, de acordo com o domain driven design é considerada um service.
