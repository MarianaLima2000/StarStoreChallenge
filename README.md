# StarStoreChallenge

StarStore
O desafio consiste em criar uma loja de itens de Star Wars que o usuário é capaz de adicionar os itens desejados em um carrinho de compras e finalizar a compra com uma simulação de transação e-commerce.

O candidato, ao finalizar, deve enviar o repositório do github para sistemas@stone.com.br para análise do time.

Para obter os itens da loja, sua aplicação deverá realizar uma chamada GET na URL https://raw.githubusercontent.com/stone-pagamentos/desafio-mobile/master/store/products.json

A lista de itens deve exibir as seguintes informações:

- Nome [title]
- Preço [price]
- Vendedor [seller]
- Foto do item [thumbnailHd]


Após o usuário adicionar todos os itens no carrinho, ele deverá finalizar a compra. Para finalizar a compra, deve realizar uma chamada POST na URL 
https://us-east1-s4hpf63bwchwcxyc8gn1op1rfij43v.cloudfunctions.net/mobile-challenge-post
com os seguintes atributos:

- Id do usuário a ser salvo as transações
- Número do cartão (máximo de 16 números - XXXX XXXX XXXX XXXX)
- Nome do portador do cartão
- Vencimento do cartão (MM/yy)
- CVV (código encontrado na parte traseira do cartão)
- Valor da transação (total dos itens no carrinho)
- Lista Itens

## Exemplo:

{  

   "id_user": 123,
   
   "card_number":"1234123412341234",
   
   "value":7990,
   
   "cvv":789,
   
   "card_holder_name":"Luke Skywalker",
   
   "exp_date":"12/24",
   
   "itens": ["Blusa do Imperio","Blusa C3-PO"]
   
}

A aplicação deverá conter uma tela para exibir as transações já feitas.
Essas transações podem ser recuperadas usando um GET no endpoint:
https://us-east1-s4hpf63bwchwcxyc8gn1op1rfij43v.cloudfunctions.net/mobile-challenge-get

Qualquer dúvida pode ser enviada pro email sistemas@stone.com.br
