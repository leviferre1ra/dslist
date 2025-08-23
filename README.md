# DSList 🎮

O **DSList** é um projeto de estudo back-end desenvolvido em **Java** com o framework **Spring Boot**, utilizando **SQL** para persistência de dados. O sistema foi projetado seguindo um modelo em **camadas**, aplicando boas práticas e padrões de projeto.

## Diagrama de Classes UML
<img width="824" height="290" alt="image" src="https://github.com/user-attachments/assets/4704b450-350b-4b3e-ad33-7dc32735b542" />


## Tecnologias utilizadas
- **Java 21**
- **Spring Boot**
- **JPA / Hibernate**
- **H2 Database** (ambiente de teste)
- **PostgreSQL** (ambiente de produção)
- **Maven**

## Funcionalidades
- Listagem de games armazenados no banco de dados.  
- Organização dos jogos em listas personalizadas.  
- Reordenação de games dentro da lista, com atualização automática no banco de dados.  
- Arquitetura baseada em:
  - Controladores REST
  - Services
  - Repositórios (JPA)
  - DTOs e Entities

## Estrutura
- **Camada de controladores (REST)** → Recebe requisições HTTP e retorna JSON.  
- **Camada de serviço** → Contém a lógica de negócios.  
- **Camada de acesso a dados (repositories)** → Comunicação com o banco via JPA/Hibernate.
![Imagem do WhatsApp de 2025-08-22 à(s) 23 29 12_85883e94](https://github.com/user-attachments/assets/f71a5d8a-bebd-4004-ae93-b884837e52a8)


## Banco de dados
O projeto foi testado com **H2 Database** e integrado ao **PostgreSQL** para ambientes reais.


## ⚙️ Como executar o projeto

### Pré-requisitos
- [Java 21+](https://www.oracle.com/java/technologies/downloads/)  
- [Maven](https://maven.apache.org/)  
- [Docker](https://www.docker.com/) (opcional, para rodar o PostgreSQL)  

---

### 🔹 Executando com banco H2 (em memória)
O projeto já vem configurado com o **H2 Database** para testes.  
Basta rodar os comandos:

```bash
# Clonar repositório
git clone https://github.com/leviferre1ra/dslist.git

# Entrar na pasta do projeto
cd dslist

# Executar aplicação
./mvnw spring-boot:run
