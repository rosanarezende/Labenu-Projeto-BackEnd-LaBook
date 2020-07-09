# Labenu | Full-Stack Web Development Bootcamp
Desenvolvimento de aplicações completas, incluindo frontend Web com React e backend com Node.js.

![Screenshot_1](https://user-images.githubusercontent.com/45580434/79641791-06e1c100-8170-11ea-8ecf-b6c889805d55.png)

<br><br>

# Backend - Projeto Labook

<br>

## Principais tecnologias/ferramentas utilizadas

1. **Node**
2. **Typescript**
3. **Arquitetura MVC**
4. **MySQL** (para construção do banco de dados)
5. **Knex** (para conexão com o banco de dados)
6. **Express** (para interação do código através do protocolo HTTP)
7. **Dotenv** (para acessar informações sensíveis por meio de variáveis de ambiente)
8. **UUID** (para geraração de id)
9. **Bcryptjs** (para criptografar senhas)
10. **Jsonwebtoken** (para gerar tokens de autenticação)
11. **Jest** (para testes automatizados)

<br>

## Escopo

Desenvolver o backend de uma rede social, o LaBook, que nasceu como uma rede de alunos de universidades americanas, e agora parece que já tem um número aceitável de usuários (2 bilhões).

A rede social tem por objetivo de promover a conexão e interação entre seus mais diversos usuários. Os usuários podem criar posts de dois tipos ("evento" ou "normal), comentá-los e curti-los também. O desenvolvedor do frontend é bastante experiente e já preparou uma lista de todos os endpoints que serão necessários para o projeto:

### Endpoints obrigatórios

1. **Cadastrar**

    Para o cadastro nessa rede social, o usuário deve fornecer seu nome, seu e-mail e uma senha. Além disso, esse endpoint já tem que realizar o login do usuário, fornecendo seu token de autenticação no retorno da requisição.

2. **Logar**

    Para realizar o login, basta informar seu e-mail e a sua senha. O retorno deve conter o token de autenticação do usuário.

3. **Fazer amizade**

    Criar uma amizade é simples: basta receber o token de autenticação junto com o Id do usuário com o qual se deseja fazer amizade. 

    Uma amizade é uma "relação mútua": quando um usuário vira amigo de outro, esse outro "já é amigo" desse primeiro usuário (ou seja, o segundo usuário não precisa virar amigo do outro depois)

    *Não há a necessidade de "aceitar" uma amizade.*

4. **Desfazer Amizade**

    Encerrar uma amizade segue o mesmo fluxo de fazer: com o token de autenticação e o id do usuário, já é possível realizar esse processo.

    Observação: você deve retornar um erro caso o usuário tente desfazer uma amizade com alguém com quem não tem essa amizade registrada no banco!

5. **Criar post**

    O post deve ser criado, passando-se as informações de: foto, descrição, data de criação e tipo ("normal" ou "evento").

6. **Ver todo o Feed**

    O feed é composto por todos os posts dos  amigos do usuário logado. Os posts devem ser retornado em ordem de criação: do mais recente ao mais antigo.

7. **Ver apenas um tipo de post do Feed**

    Esse endpoint deve receber um tipo ("normal" ou "evento") e retornar todos os posts que sejam do tipo especificado. Os posts devem ser retornado em ordem de criação: do mais recente ao mais antigo.

<br>

Por fim, ressaltam-se dois fatos:

- Você deve analisar e pensar quais são os endpoints que necessitam do token de autenticação
- Lembre-se de que o Backend deve ser muito conciso. Isso significa que você deve prever a maior parte dos erros que possam acontecer e já se precaver contra eles. (Não se preocupe muito com essa parte, mas, se der tempo, foque nisso!)

<br>

### Desafios

8. **Curtir Post**

    Essa requisição deve receber somente o id do post e retornar uma mensagem de sucesso ou erro. Lembre-se de que um usuário não pode curtir o mesmo post duas vezes.

9. **Descurtir Post**

    Essa requisição deve receber somente o id do post e retornar uma mensagem de sucesso ou erro. Lembre-se de que um usuário não pode descurtir um post que não tenha curtido

10. **Comentar Post**

    Recebendo o id do post e mensagem do comentário, o endpoint deve funcionar sem problemas. Um usuário pode, se quiser, comentar mais de uma vez o mesmo post. 

11. **Implemente a funcionalidade que permita que o token de autenticação seja atualizado**

    Também conhecido como "Refresh Token", você deve implementar um endpoint que permita que o Frontend autalize o "acess token", caso este expire

<br>

## Como rodar a aplicação

No terminal, clone o projeto:
```
git clone 
```

Entre na pasta do projeto:
```
cd Labenu-Projeto-BackEnd-LaBook/app
```

Instale as dependências:
```
npm install
```

Execute a aplicação:
```
npm start 
```

<br>

## Contribuição

Contribuições com o projeto são muito apreciadas. Para isso:

- Faça um Fork do projeto

- Crie uma branch para sua feature
```
git checkout -b feature
```

- Adicione as mudanças
```
git add . 
```

- _Commit_ as mudanças 
```
git commit -m 'Adicionando a feature X'
```

- Faça o push da branch 
```
git push origin feature
```

- Abra um Pull Request

<br>

## Licença

The [MIT License]() (MIT)

Copyright :copyright: 2020 - 4eddit

<br>

## Canais de comunicação

**Rosana-Rezende**: *Desenvolvedora web full-stack | Advogada | MBA em gestão: inteligência de negócios digitais - FGV*

- [Linkedin](https://www.linkedin.com/in/rosanarezende/)
- [Github](https://github.com/rosanarezende)
- [Email](rezende_rosana@hotmail.com)

<br>

## Desenvolvedores/Contribuintes :octocat:

<div align="center">

| [<img src="https://avatars1.githubusercontent.com/u/59854938?s=460&u=354eee3f994ad58a87ad021204151755f6e2538b&v=4" width=115><br><sub>Marina Isabel</sub>](https://github.com/marinaisabels) |  [<img src="https://avatars2.githubusercontent.com/u/58155127?s=460&u=669a5b9c80a44d3ba2834ecd3d2de8bae3d950db&v=4" width=115><br><sub>Thales Fernando Milanezi</sub>](https://github.com/ThalesMilanezi) |  
| :---: | :---: 

</div>
