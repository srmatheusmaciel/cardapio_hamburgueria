# Cardápio Hamburgueria

## Visão Geral
O **Cardápio Hamburgueria** é uma API desenvolvida para gerenciar um cardápio online, permitindo que clientes escolham seus pedidos e os enviem diretamente para a empresa via WhatsApp. O sistema utiliza um banco de dados SQLite3 para armazenar os produtos, mas não armazena os pedidos.

## Funcionalidades
- Listar os itens do cardápio com detalhes (nome, descrição, preço)
- Adicionar novos itens ao cardápio
- Editar e remover itens do cardápio
- Estilização responsiva com Tailwind CSS
- API que envia o pedido diretamente para um número de WhatsApp cadastrado

## Tecnologias Utilizadas
- **Node.js**: Ambiente de execução JavaScript do lado do servidor
- **Express**: Framework para facilitar a criação do servidor
- **SQLite3**: Banco de dados leve e eficiente para armazenar os produtos do cardápio
- **Tailwind CSS**: Framework CSS para estilização rápida e responsiva


## Instalação e Execução
### Pré-requisitos
- Node.js instalado (versão 14+)
- NPM ou Yarn

### Passos para rodar o projeto
1. Clone o repositório:
   ```sh
   git clone https://github.com/seu-usuario/cardapio_hamburgueria.git
   cd cardapio_hamburgueria
   ```
2. Instale as dependências:
   ```sh
   npm install
   ```
3. Inicie o servidor:
   ```sh
   npm start
   ```
4. Acesse a API no navegador ou no Postman:
   ```sh
   http://localhost:3000
   ```

## Endpoints da API
| Método | Rota              | Descrição                          |
|--------|-------------------|------------------------------------|
| GET    | `/api/menu`       | Retorna todos os itens do cardápio |
| GET    | `/api/menu/:id`   | Retorna um item específico        |
| POST   | `/api/menu`       | Adiciona um novo item ao cardápio |
| PUT    | `/api/menu/:id`   | Atualiza um item existente        |
| DELETE | `/api/menu/:id`   | Remove um item do cardápio        |

## Envio de Pedido pelo WhatsApp
Quando um cliente escolhe um pedido, a API gera um link que redireciona automaticamente para o WhatsApp com a mensagem do pedido pré-preenchida. O número do WhatsApp deve ser configurado no código.

## Contribuição
Sinta-se à vontade para contribuir com melhorias no projeto:
1. Fork este repositório
2. Crie uma branch para sua feature (`git checkout -b feature-nova`)
3. Faça o commit das alterações (`git commit -m 'Adiciona nova funcionalidade'`)
4. Envie para o repositório (`git push origin feature-nova`)
5. Abra um Pull Request

## Licença
Este projeto está licenciado sob a **MIT License**.

