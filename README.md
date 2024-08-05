# StarStoreChallenge

StarStore
O desafio consiste em criar uma loja de itens de Star Wars que o usuário é capaz de adicionar os itens desejados em um carrinho de compras e finalizar a compra com uma simulação de transação e-commerce.

O desafio deve ser feito utilizando React Native + TypeScript

O candidato, ao finalizar, deve enviar o repositório do github para mariana.brito@stone.com.br para análise do time.

## Itens da Loja
Para obter os itens da loja, sua aplicação poderá realizar uma chamada GET na [URL](https://raw.githubusercontent.com/stone-pagamentos/desafio-mobile/master/store/products.json),
É um diferencial utilizar um back-end próprio com uso de um banco de dados sem a utilização dessa rota.

A lista de itens deve exibir as seguintes informações:

- Nome [title]
- Preço [price]
- Vendedor [seller]
- Foto do item [thumbnailHd]

## Carrinho
Após o usuário adicionar todos os itens no carrinho, ele deverá finalizar a compra. Para finalizar a compra, deve receber e salvar no cache do app as seguintes informações:

- Id do usuário a ser salvo as transações
- Número do cartão (máximo de 16 números - XXXX XXXX XXXX XXXX)
- Nome do portador do cartão
- Vencimento do cartão (MM/yy)
- CVV (código encontrado na parte traseira do cartão)
- Valor da transação (total dos itens no carrinho)
- Lista Itens

## Histórico de compras
A aplicação deverá conter uma tela para exibir as transações já feitas.
Essas transações podem ser recuperadas do próprio cache do app utilizando o storage ou algum back-end (podendo ser utilizado firebase, caso queira).

## Layout
A aplicação deve seguir o [layout](https://www.figma.com/file/ioHxpFUcGdWcfZxgFwasIR/StarStore?node-id=0%3A1) como projetado no figma.

## Diferenciais
São diferenciais, porém não obrigatório, o uso de:

- Redux
- Uso de styled-components
- Uso de AsyncStorage para persistência
- Back-end próprio hospedado em infraestrutura de nuvem
- Ferramentas de log e monitoramento
- Padrão de projeto claro e explicado no README
- Autenticação com uso das principais plataformas (google, facebook, apple)
- Sugestões de novas funcionalidades que se adequem ao projeto


Qualquer dúvida pode ser enviada pro email mariana.brito@stone.com.br
