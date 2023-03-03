[![NPM](https://img.shields.io/npm/l/react)](https://github.com/lucarauj/criacao-de-API-parking-control-com-Java-Spring-Security/blob/main/LICENSE)

<p align="center"><img width="200px" src="https://github.com/lucarauj/assets/blob/main/ApiJavaSpring.png" /></p>

<h1 align="center"> Spring Security na API Parking Control com Java: </h1>
<h2 align="center"> Controle de Acesso </h2>

### 👉 [LINK DO PROJETO BASE 🖱](https://github.com/lucarauj/criacao-de-API-parking-control-com-Java)

<br>

- ✅ Versão utilizada: Spring boot: 2.6.3 / Spring boot Security: 2.6.3

- ❌ Top 10 Vulnerabilidades de Segurança em Aplicações Web: https://owasp.org/www-project-top-ten/

<br>

- 401 Unauthorized: usuário não logado; precisa enviar as credenciais corretas de acesso;
- 403 Forbidden: usuário logado mas não autorizado a acessar recurso específicos;

<br>

- ⚙ Configurando arquivo ```pom.xml```:

```
<dependency>
	<groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-security</artifactId>
	<version>2.6.3</version>
</dependency>
```


- 🛒 Populando o banco de dados com um Usuário:

```
insert into tb_user values('uuid', 'encode', 'marta');
```

- ☢ UUID: https://www.uuidgenerator.net/
- ☢ gen_random_uuid()
- ☢ System.out.println(new BCryptPasswordEncoder().encode("senha123"));

<br>

- 🛒 Populando o banco de dados com um Perfil de Usuário:

```
insert into tb_role values(gen_random_uuid(), 'ROLE_ADMIN');
insert into tb_role values(gen_random_uuid(), 'ROLE_USER');
```
```
insert into tb_users_roles values('inserir uuid Marta', 'inserir uuid Admin')
insert into tb_users_roles values('inserir uuid Bruno', 'inserir uuid User')
```

### 📝 Mais anotações utilizadas no projeto:

- @Configuration: define uma classe como fonte de definições de beans;
- @Bean: utilizada em métodos de uma classe, geralmente marcada com @Configuration, indicando ao Spring Framework que deve invocar aquele método e gerenciar o objeto retornado por ele;
- @Entity: utilizada para informar que uma classe também é uma entidade;
- @Table: usada para especificar a tabela principal da entidade atualmente anotada;
- @Id: especifica o identificador da entidade, que é usado ao carregar a entidade em um determinado contexto de persistência;
- @GeneratedValue(strategy = GenerationType.AUTO)
- @Column: usada para especificar o mapeamento entre um atributo de entidade básico e a coluna da tabela de banco de dados;
- @Repository: serve para definir uma classe como pertencente à camada de persistência;
- @Service: marca uma classe Java que executa algum serviço;
- @Autowired: delega ao Spring Boot a inicialização do objeto;
- @Enumerated(EnumType.STRING): armazena na coluna do parâmetro na tabela a String que representa a constante da enumeração;
- @ManyToMany: este relacionamento informa que muitos registros de uma entidade estão relacionados com muitos registros de outra entidade;
- @JoinTable: define o nome de uma tabela;
- @JoinColumn: define o nome dos campos;
- @Transactional: utilizada nos métodos que precisam de transação;
- @EnableGlobalMethodSecurity: usada para habilitar o uso das anotações com as regras de segurança
- @PreAuthorize: verifica a expressão dada antes de inserir o método

## 🚀 Tecnologias

Esse projeto foi desenvolvido com as seguintes tecnologias:
<div style="display: inline_block"><br>
<img align="center" alt="Lucarauj-Java" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg">
<img align="center" alt="Lucarauj-Postman" height="50" width="90" src="https://github.com/lucarauj/assets/blob/main/postman.png">
<img align="center" alt="Lucarauj-Spring" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/spring/spring-original.svg">
<img align="center" alt="Lucarauj-Postgresql" height="40" width="50" src="https://github.com/lucarauj/assets/blob/main/postgresql.svg">
</div>

## Aluno

Lucas Araujo

<a href="https://www.linkedin.com/in/lucarauj"><img alt="lucarauj | LinkdeIN" width="40px" src="https://user-images.githubusercontent.com/43545812/144035037-0f415fc7-9f96-4517-a370-ccc6e78a714b.png" /></a>

