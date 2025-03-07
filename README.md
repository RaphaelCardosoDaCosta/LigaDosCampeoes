# Champions League Manager

Sistema web desenvolvido em **Java**, utilizando **JSP, Servlets, MySQL e Tomcat**, para gerenciar clubes e jogadores da Champions League.

## 🚀 Funcionalidades
- **Gestão de Clubes:** Criar, visualizar, editar e excluir clubes.
- **Gestão de Jogadores:** Cadastrar, listar e associar jogadores a clubes.
- **Banco de Dados MySQL:** Armazena clubes e jogadores com relacionamento entre as tabelas.
- **Interface Web com JSP:** Exibição dinâmica dos dados e formulários para interação.

## 🛠️ Tecnologias Utilizadas
- **Java (JSP & Servlets)** - Processamento das requisições.
- **MySQL** - Armazenamento de dados.
- **Tomcat** - Servidor de aplicação.


## ⚙️ Configuração do Ambiente
1. Instale o **JDK 11+** e o **Apache Tomcat**.
2. Configure um banco MySQL e crie as tabelas:
   ```sql
   CREATE TABLE clubes (
       id INT AUTO_INCREMENT PRIMARY KEY,
       nome VARCHAR(100) NOT NULL,
       pais VARCHAR(50) NOT NULL,
       ano_fundacao INT NOT NULL
   );

   CREATE TABLE jogador (
       
       nome VARCHAR(100) NOT NULL,
       clube VARCHAR(1OO) NOT NULL,
       nac VARCHAR(50) NOT NULL,
       camisa INT NOT NULL,
       posicao VARCHAR(50) NOT NULL,
       id INT AUTO_INCREMENT PRIMARY KEY,
   );
   ```
3. Configure a conexão no arquivo DAO.
4. Importe o projeto em uma IDE como **Eclipse** ou **IntelliJ IDEA**.
5. Execute o **Tomcat** e acesse `http://localhost:8080/ChampionsLeagueManager/`.


