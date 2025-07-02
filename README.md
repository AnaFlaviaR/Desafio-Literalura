# 📚 Catálogo de Livros - Projeto LiterAlura

Este projeto é um **catálogo interativo de livros** desenvolvido em **Java** com **Spring Boot**, que permite buscar livros através da API pública **Gutendex**, salvá-los em um banco de dados e realizar consultas por meio de uma interface textual (console).

---

## 🚀 Funcionalidades

- 🔎 **Buscar livro por título**
- 📚 **Listar todos os livros buscados**
- 👨‍💼 **Listar autores dos livros buscados**
- 🧓 **Listar autores vivos em determinado ano**
- 🌍 **Exibir quantidade de livros por idioma**

---

## 🛠️ Tecnologias Utilizadas

- Java 21
- Spring Boot 3
- Spring Data JPA
- H2 Database (memória)
- Maven
- Jackson (JSON)
- HttpClient (Java 11+)
- API: [Gutendex](https://gutendex.com/)

---

## 📦 Como executar o projeto

### Pré-requisitos:
- Java 21+
- Git
- (Opcional) IDE: IntelliJ, VS Code, Eclipse...

### Passos:

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/catalogo-livros.git
cd catalogo-livros
```

2. Compile o projeto com Maven:
```bash
./mvnw clean package
```
(Windows: `mvnw.cmd clean package`)

3. Execute o `.jar`:
```bash
java -jar target/literalura-0.0.1-SNAPSHOT.jar
```

---

## 💾 Banco de dados

- Utiliza banco H2 em memória.
- Console do H2 habilitado: `http://localhost:8080/h2-console`
- JDBC URL: `jdbc:h2:mem:livrosdb`

---

## 🧠 Sobre a API Gutendex

A API [Gutendex](https://gutendex.com/) fornece acesso aos dados de mais de 70 mil livros gratuitos do Projeto Gutenberg. Este projeto usa:

- `/books/?search={titulo}` para buscar livros por título
- Dados extraídos: título, autor, idioma e número de downloads

---

## 👤 Autora

Ana Flavia de Sousa Reis  
💻 Apaixonada por tecnologia, focada em back-end e APIs REST.

---

## 📝 Licença

Este projeto é de uso educacional, baseado no desafio do curso *LiterAlura* da plataforma Alura.
