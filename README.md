<h1 align="center">Docker Manager Java</h1>

### 💻 Sobre o Projeto

O **Docker Manager** é uma API REST desenvolvida em Java que se comunica com a API do Docker Daemon.  
Ela oferece uma interface simples e eficiente para gerenciar containers, imagens e recursos Docker diretamente via chamadas HTTP.

### ⚙️ Funcionalidades

- [x] **Gerenciar containers:**
  - Criar, listar, iniciar, parar, reiniciar e remover containers.
- [x]  **Gerenciar imagens Docker:**
  - Listar imagens Docker locais com ou sem filtros.

### 📄 Endpoints

| Método  | Endpoint                            | Descrição                                                                |
|---------|-------------------------------------|--------------------------------------------------------------------------|
| `GET`   | `/api/images`                       | Lista todas as imagens Docker disponíveis.                               |
| `GET`   | `/api/images?filterName=<nome>`     | Lista imagens Docker que correspondem ao filtro informado.               |
| `GET`   | `/api/containers?showAll=true`      | Lista todos os containers, incluindo os parados.                         |
| `GET`   | `/api/containers?showAll=false`     | Lista apenas os containers em execução.                                  |
| `POST`  | `/api/containers`                   | Cria um novo container com base na imagem especificada.                  |
| `POST`  | `/api/containers/{id}/start`        | Inicia um container pelo ID.                                             |
| `POST`  | `/api/containers/{id}/stop`         | Para um container pelo ID.                                               |
| `DELETE`| `/api/containers/{id}`              | Remove um container pelo ID.                                             |


### 🛠 Tecnologias

As seguintes ferramentas e bibliotecas foram utilizadas no desenvolvimento do projeto:

- [Java](https://www.java.com/)
- [Spring Boot](https://spring.io/projects/spring-boot)
- [Java Docker API Client](https://github.com/docker-java/docker-java)

### 👨🏼‍💻 Autor

William Dias Marcos

 <a href = "mailto:william.diasmarcos@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white"        target="_blank"></a>
 <a href="https://www.linkedin.com/in/william-dias-marcos-25981a192" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>
