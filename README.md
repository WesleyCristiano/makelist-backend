# MakeList.com.br
- A aplicação consiste em uma papelaria online onde será possível ao cliente realizar a compra da lista de materiais de seu filho.

- A experiência de compra será feita de maneira personalidade, ou seja, para cada cliente serão apresentados os produtos de acordo com a lista esolhida, fazendo com que o cliente não perca tempo pesquisando os produtos. 

## Fluxo do cliente na loja

- A página inicial o cliente escolherá a escola e a série que seu filho estuda. Ao fazer isso será redirecionado para as páginas seguintes, onde em cada página escolherá os produtos na ordem em que são solicitados na lista de materiais de seu filho. 

- Ao final da lista, também será possível ao cliente comprar outros produtos da papelaria para seu filho que eventualmente não estão na lista de materias, como mochilas, estojos etc.

- Após o cliente será redirecionado para a página de carrinho, onde poderá:

    **1)** conferir a lista do produtos escolhidos.

    **2)** escolher a forma de entrega (receber no endereço deseja ou retirar na loja).

    **3)** realizar login ou criar uma conta caso não possua uma. 

    **4)** escolher a forma de pagamento (cartão de crédito/ boleto bancário /transferência)

- Após realizar o pagamento o cliente será redirecionado para uma página de obrigado com informações do pedido (número do pedido, status)

- Ao final o cliente receberá um email de confirmação de pedido.

## Fluxo do lojista na plataforma

- Após o cliente finalizar o pedido o lojista será notificado (email/notificação).

- Após a migração do pedido para o status "pagamento confirmado" o lojista imprimirá a lista de itens do pedido para a separação.

- Após a separação o lojista providenciará a entrega dos produtos (retirada ou entrega em endereço) e atualizará o status para 'produtos enviados' ou 'produto disponíveis para retirada'.

- Após a entrega o lojista deverá realizar a finalização do pedido anexando comprovante de entrega na plataforma(foto/pdf) e alterará o status para entregue.

- Ao cliente finalizar o pedido o lojista:

    **1)** vizualizará o pedido em sua Dashoboard com os possíveis status(Pedido Recebido ou Pagamento confirmado

    **2)** após a confirmação do pagamento, imprimirá o pedido para a separação (relatório pdf).

    **3)** Realizará a entrega do pedido (ou retirada)

## Schema Visual do [Banco de Dados](https://whimsical.com/PZSTqGP7fPPR9m2iDRe66A)


## Rotas da aplicação

   - **`POST/products/`**: Esta rota deve fazer o cadastro de produtos da aplicação.

   - **`POST/stores/`**: Esta rota deve fazer o cadastro da papelarias.

   - **`POST/categories/`**: Esta rota deve fazer o cadastro de categorias da aplicação

   - **`POST/lists/`**: Esta rota deve fazer o cadastro de listas de materiais.

   - **`POST/schools/`**: Esta rota deve fazer o cadastro de escola.

   - **`GET/stores/cities`**: Retorna todas as cidades que contém pelo menos uma loja.

   - **`GET/schools/cities?city={city}&state={state}`**: Retorna todas as escolas em determinada cidade.

   - **`GET/lists/:school_id`**: Retorna todas as listas de uma determinada escola.

   - **`GET/lists/:list_id?/products?STORE_ID={STORE_ID}`**: Retorna todas as listas de uma determinada escola.

   - **`PATCH/products/:product_id/images`**: Esta rota deve fazer ser capaz de incluir/atualizar as images do produto.












     
      



      
   
   
      
      
