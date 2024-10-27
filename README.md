# API de Conversão de Moeda

Esta API simples realiza a conversão de moeda com base em uma taxa fornecida.

## Como usar

A API pode ser acessada através da seguinte URL: localhost:8000

/exchange/{valor}/{moeda_origem}/{moeda_destino}/{taxa}

Onde:

* `{valor}` é o valor a ser convertido.
* `{moeda_origem}` é o código da moeda de origem (ex: BRL).
* `{moeda_destino}` é o código da moeda de destino (ex: USD).
* `{taxa}` é a taxa de câmbio.

**Exemplo:**

Para converter 10 reais para dólares americanos com uma taxa de 4.5, a URL seria:
exchange/10/BRL/USD/4.5

## Resposta

A API retorna um JSON com o seguinte formato:

```json
{
  "valorConvertido": 45.00,
  "simboloMoeda": "$"
}

Análise concluída

Aqui está um exemplo de arquivo README.md que você pode usar:

Markdown
# API de Conversão de Moeda

Esta API simples realiza a conversão de moeda com base em uma taxa fornecida.

## Como usar

A API pode ser acessada através da seguinte URL:

Use o código com cuidado.

/exchange/{valor}/{moeda_origem}/{moeda_destino}/{taxa}


Onde:

* `{valor}` é o valor a ser convertido.
* `{moeda_origem}` é o código da moeda de origem (ex: BRL).
* `{moeda_destino}` é o código da moeda de destino (ex: USD).
* `{taxa}` é a taxa de câmbio.

**Exemplo:**

Para converter 10 reais para dólares americanos com uma taxa de 4.5, a URL seria:

/exchange/10/BRL/USD/4.5


## Resposta

A API retorna um JSON com o seguinte formato:

```json
{
  "valorConvertido": 45.00,
  "simboloMoeda": "$"
}
Onde:

valorConvertido é o valor convertido.
simboloMoeda é o símbolo da moeda de destino.
Códigos de Erro
Em caso de erro, a API retorna um código de erro HTTP e um JSON com uma mensagem de erro.

Exemplos:

400 Bad Request: Formato de URL inválido ou moeda inválida.
JSON
{
  "error": "Formato de URL inválido"
}
Use o código com cuidado.

JSON
{
  "error": "Moeda destino inválida: XYZ"
}
Use o código com cuidado.

Testes
Os testes unitários podem ser executados usando o PHPUnit:

phpunit --bootstrap src/ExchangeController.php tests/ExchangeControllerTest.php
Lint
O código pode ser verificado usando o PHP CodeSniffer:

phpcs --standard=PSR12 src/
Correção de Lint
O código pode ser corrigido automaticamente usando o PHP Code Beautifier and Fixer:

phpcbf --standard=PSR12 src/
Observações
A API suporta as seguintes moedas: USD, BRL e EUR.
As taxas de câmbio são fornecidas pelo usuário e podem não refletir as taxas atuais do mercado.

Para contato: renebmjr@gmail.com
