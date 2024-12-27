# Esquema_Conceitual_BcoDados_ECommerce
Desafio Ecommerce - DIO: Esquema do Projeto Conceitual do Banco de Dados

O projeto conceitual do banco de dados Ecommerce inclui várias entidades principais, sendo que no esboço inicial tinha essas 6 entidades: Cliente, Produto, Fornecedor, VendedorExterno|Terceiro, Estoque, Pedido. 

No refinamento, inclui no esquema 3 outras entidades: Entrega, Pagamento e Cancelamento do Pedido. 

Cada entidade possui atributos específicos que descrevem suas características, no caso refinei a configuração de cada uma delas conforme suas particularidades e intenções.

Pontuo a necessidade de validar com negócios cada termo e regra utilizada:
- Documento Cliente é apenas um campo em que poderá ser preenchido com CPF ou CNPJ. Neste caso a plataforma terá que validar o documento preenchido.
- Status Pedido('Pendente', 'Concluído', 'Cancelado');
- Status Entrega('Aguardando Envio', 'Em transito', 'Entregue', 'Devolvido');
- Método Pagamento('PIX', 'Cartão de Débito', 'Cartão de Crédito à vista', 'Cartão de Crédito parcelado 10 vezes sem juros');
- Status Pagamento('Pendente', 'Pago', 'Estornado')

Além disso, há relacionamentos entre essas entidades apresentados no esquema conceitual que ajudam a estruturar e organizar os dados, sendo que em alguns casos são do tipo:
- 1:1;
- 1:n;
- n:m (esses são 4: Produtos por Fornecedor, Produtos por Vendedor Externo| Terceiro, Produto em Estoque, Relação de Produto/Pedido).
