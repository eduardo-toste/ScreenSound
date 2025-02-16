# ScreenSound

## Sobre o Desafio
Este projeto tem como objetivo desenvolver uma aplicação para armazenar informações sobre artistas e músicas em um banco de dados relacional. A aplicação permitirá o cadastro de artistas e suas músicas, além de consultas para facilitar a organização e recuperação dessas informações.

## Funcionalidades
- Cadastrar artistas e suas músicas no banco de dados;
- Pesquisar músicas por artista;
- Utilizar um enum para definir o tipo do artista (solo, dupla ou banda);
- Utilizar Spring Data JPA para gerenciar os dados no PostgreSQL.

## Tecnologias Utilizadas
- Java + Spring Boot (Spring Data JPA, PostgreSQL, Spring Web);
- Banco de Dados Relacional (PostgreSQL);
- Spring Initializr (Criação do projeto e gerenciamento de dependências).

## Estrutura do Projeto
- **Classe `Artista`**: Representa um artista e contém atributos como nome, gênero musical e tipo (solo, dupla ou banda);
- **Classe `Musica`**: Representa uma música associada a um artista;
- **Relacionamento**: Um artista pode ter várias músicas (OneToMany);
- **Menu Interativo**: Criado na classe principal, permitindo interação via terminal;
- **CommandLineRunner**: Implementado para inicializar o menu ao iniciar a aplicação.

## Como Executar o Projeto
1. Clone este repositório:
   ```bash
   git clone https://github.com/eduardo-toste/ScreenSound.git
   ```
2. Acesse o diretório do projeto:
   ```bash
   cd ScreenSound
   ```
3. Configure o banco de dados PostgreSQL no `application.properties`;
4. Compile e execute o projeto:
   ```bash
   mvn spring-boot:run
   ```

## Contribuição
Contribuições são bem-vindas. Faça um fork do projeto, crie uma branch com suas alterações e envie um pull request.
