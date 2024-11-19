# UserAuth API - Gestão de Usuários Segura

Bem-vindo ao repositório do **UserAuth API**, uma API desenvolvida com [NestJS](https://nestjs.com/) para autenticação e gestão de usuários, utilizando as melhores práticas do mercado. Este projeto oferece uma base sólida e escalável, usando **Identificadores Globais Únicos (UUIDs)** para identificação de usuários e entidades, garantindo maior segurança e flexibilidade.

## Recursos

- **Autenticação Segura**:  
  Implementação de autenticação baseada em tokens JWT (JSON Web Token).  

- **Identificadores Globais Únicos (UUIDs)**:  
  Identificação de usuários e registros com UUIDs para evitar vulnerabilidades associadas a IDs incrementais.

- **Estrutura Modular**:  
  Arquitetura modular do NestJS para fácil expansão e manutenção.

- **Gerenciamento de Usuários**:  
  Rotas para cadastro, login, recuperação de senha e edição de perfil.

- **Segurança**:  
  Proteção de rotas com *Guards* e estratégias customizadas.

## Tecnologias Utilizadas

- **NestJS**: Framework para construção de APIs escaláveis e robustas.
- **TypeScript**: Linguagem principal do projeto.
- **TypeORM**: Para integração e manipulação de banco de dados.
- **PostgreSQL**: Banco de dados relacional.
- **Passport**: Estratégia de autenticação.
- **JWT**: Tokens seguros para autenticação.

## Endpoints Principais

### Rotas Públicas
- **POST** `/auth/register`  
  Cadastro de novos usuários.  

- **POST** `/auth/login`  
  Login de usuários para obtenção do token JWT.

### Rotas Protegidas
- **GET** `/users/profile`  
  Consulta os dados do perfil do usuário autenticado.  

- **PATCH** `/users/profile`  
  Atualiza informações do perfil do usuário autenticado.  

- **POST** `/auth/forgot-password`  
  Gera link para recuperação de senha.

- **POST** `/auth/reset-password`  
  Permite redefinir a senha com base no token gerado.

## Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/userauth-api.git


2. Instale as dependências:
   ```bash
   npm install

3. Configure as variáveis de ambiente:
Crie um arquivo .env com as seguintes configurações:
   ```bash
    DATABASE_URL=postgres://usuario:senha@localhost:5432/nome_banco
    JWT_SECRET=sua_chave_secreta
    PORT=3000
   
Inicie o servidor:
   ```bash
   npm run start:dev

Contribuindo
Sinta-se à vontade para contribuir com melhorias ou abrir issues! Este projeto foi criado para ser uma base de aprendizado e colaboração.

Licença
Distribuído sob a licença MIT. Consulte o arquivo LICENSE para mais informações.
