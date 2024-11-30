# ProjetoJavaSemestre

# Sistema de Gerenciamento de Restaurantes e Usuários

Este projeto foi desenvolvido para gerenciar usuários e restaurantes participantes de um programa de doação de alimentos. O sistema foi implementado em Java, utilizando banco de dados MySQL, e segue uma estrutura organizada com classes e métodos específicos para cada funcionalidade.

## Funcionalidades do Sistema

### 1. Gerenciamento de Usuários
- Cadastro de usuários com validação de dados.
- Login com autenticação baseada no banco de dados.
- Exclusão de usuários, incluindo validação por senha.

### 2. Gerenciamento de Restaurantes
- Cadastro de restaurantes com informações detalhadas:
  - Nome, telefone, dias de atendimento.
  - Endereço completo: rua, número, complemento, bairro, cidade, UF, e país.
- Listagem de todos os restaurantes cadastrados.
- Exclusão de restaurantes por ID, com verificação no banco de dados.

### 3. Submenu para Usuários Logados
- Acesso a funcionalidades específicas após login:
  - Visualizar informações sobre o programa.
  - Cadastrar novos restaurantes.
  - Listar e excluir restaurantes.

## Estrutura do Projeto

### Pacotes e Classes
1. **Logica**
   - `CadastroRestaurante`: Gerencia o cadastro e a persistência de restaurantes e seus endereços.
   - `Endereco`: Representa o modelo de endereço.
   - `Usuario`: Lida com o cadastro, login e exclusão de usuários.
   - `Menu`: Interface inicial para interação com o usuário.
   - `SubmenuLogado`: Interface para funcionalidades de usuários logados.
2. **Conexao**
   - `ConexaoBanco`: Gerencia a conexão com o banco de dados.

### Banco de Dados
- O sistema utiliza MySQL como banco de dados relacional.
- Tabelas:
  - `usuario`: Armazena informações de usuários.
  - `restaurante`: Armazena dados básicos de restaurantes.
  - `endereco`: Relaciona os endereços aos restaurantes.

## Requisitos do Sistema

- **Linguagem**: Java 8 ou superior.
- **Banco de Dados**: MySQL.
- **IDE**: IntelliJ (ou qualquer outra IDE compatível com projetos Java).

## Como Executar o Sistema

1. Configure o banco de dados MySQL:
   - Crie o banco de dados `ProjetoJava`.
   - Crie as tabelas necessárias (ver código SQL no projeto, se aplicável).
   - Adicione o driver caso necessário.
2. Atualize as credenciais no arquivo `ConexaoBanco`:
   - Substitua `USUARIO` e `SENHA` pelas credenciais do seu MySQL.
3. Compile e execute o projeto:
   - Abra o projeto em sua IDE favorita.
   - Execute a classe `Menu` para iniciar o sistema.

## Demonstração

### Passos para Utilizar o Sistema
1. **Cadastro de Usuário**:
   - Insira nome, email, username e senha.
2. **Login**:
   - Use o username e senha cadastrados.
3. **Acesso ao Submenu**:
   - Escolha entre cadastrar restaurantes, listar restaurantes ou excluir um restaurante.
4. **Exclusão de Usuário**:
   - Confirme a senha para remover o usuário do sistema.

## Colaboradores

- Marcos Vinícius dos Santos: Desenvolvimento de funcionalidades principais e integração com o banco de dados.
- Guilherme Jow Warikoda: Auxílio na estruturação do código, construção de menus, testes, e validação de dados.

## Considerações Finais

Este projeto foi desenvolvido como parte de uma atividade acadêmica para demonstrar habilidades em Java, manipulação de banco de dados e desenvolvimento de sistemas interativos. Ele pode ser expandido para incluir funcionalidades adicionais, como relatórios e integração com APIs.

---

**Agradecemos por acompanhar este projeto!**
