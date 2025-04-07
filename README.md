# Sistema de Compras Coletivas

Projeto desenvolvido para a disciplina de Web III utilizando o framework Laravel.
O objetivo é organizar compras coletivas realizadas por moradores de um grupo, gerenciando pedidos, produtos e pagamentos.

📚 Descrição do Projeto

Este sistema permite:

Cadastro de moradores (residents)

Cadastro de produtos disponíveis (products)

Registro de compras coletivas feitas pelo grupo (collective_purchases)

Associação entre pedidos de moradores e produtos (orders)

Controle de pagamentos por pedido (payments)

🧱 Estrutura do Banco de Dados

O sistema possui 5 tabelas principais com relacionamentos:

residents: moradores cadastrados

products: produtos comprados em atacado

collective_purchases: compras feitas em grupo

orders: pedidos individuais vinculados às compras coletivas

payments: status e dados de pagamento de cada pedido

Todos os relacionamentos estão definidos nas migrations usando foreignId()->constrained()->onDelete('cascade').
Os Models possuem os métodos de relacionamento apropriados: hasOne, hasMany, belongsTo, belongsToMany.

🛠️ Como Executar o Projeto

Clonar o repositório

1. git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio

2. Subir com Laravel Sail (Docker)

./vendor/bin/sail up -d

3. Instalar dependências

./vendor/bin/sail composer install

4. Rodar as migrations

./vendor/bin/sail artisan migrate

🗺️ Diagrama do Banco de Dados

![Image](https://github.com/user-attachments/assets/c64bb1e8-83a3-4b89-8840-f79badcf69bd)


✅ Requisitos Atendidos

✔ Mínimo de 5 tabelas com relacionamentos✔ Relacionamentos definidos nas migrations com foreignId e onDelete('cascade')✔ Models com relacionamentos (hasMany, belongsTo, etc.)✔ Uso de $fillable e $casts✔ Código funcionando ao rodar php artisan migrate✔ Diagrama entregue

👥 Desenvolvedores

Vinicius

Nara

Iuri
