# Sistema de Gestão de Clínica Médica

Este é um projeto de aplicação web para a gestão de uma clínica médica, permitindo o cadastro e gerenciamento de médicos e pacientes.

## 🚀 Sobre o Projeto

A aplicação foi desenvolvida utilizando a tecnologia Java Servlets para o backend e HTML para o frontend. É um sistema simples, mas funcional, que demonstra os conceitos básicos de uma aplicação web com persistência de dados.

### ✨ Funcionalidades

*   Cadastro de Pacientes
*   Cadastro de Médicos
*   Listagem de Pacientes (potencial)
*   Listagem de Médicos (potencial)

## 🛠️ Tecnologias Utilizadas

*   **Backend:** Java
    *   Java Servlets
    *   JDBC para conexão com banco de dados
*   **Frontend:** HTML
*   **Servidor de Aplicação:** Apache Tomcat (ou similar)
*   **Build:** Apache Ant (integrado com NetBeans)

## ⚙️ Como Executar o Projeto

1.  **Pré-requisitos:**
    *   JDK (Java Development Kit)
    *   Apache Tomcat (ou outro contêiner de servlets)
    *   Um banco de dados (a ser configurado no `conexãoFactory.java`)
    *   IDE NetBeans (recomendado, pois o projeto está configurado para ele)

2.  **Configuração:**
    *   Clone ou faça o download deste repositório.
    *   Abra o projeto na IDE NetBeans.
    *   Configure a conexão com o banco de dados no arquivo `src/java/br/com/clinica/servlet/connection/conexãoFactory.java`, atualizando a URL, usuário e senha.
    *   Certifique-se de que o driver JDBC do seu banco de dados esteja no classpath do projeto.

3.  **Execução:**
    *   Configure o Apache Tomcat como o servidor de aplicação no NetBeans.
    *   Execute (ou "deploy") o projeto a partir da IDE.
    *   A aplicação estará disponível no seu navegador, geralmente em um endereço como `http://localhost:8080/NOME_DO_PROJETO/`.

## 📂 Estrutura do Projeto

```
/
├── src/java/         # Código-fonte Java
│   └── br/com/clinica/
│       ├── servlet/
│       │   ├── connection/ # Classes de conexão com o BD
│       │   ├── dao/        # Data Access Objects
│       │   └── model/      # Classes de modelo (entidades)
│       └── servlets/       # Servlets que controlam as requisições
├── web/              # Arquivos da aplicação web (frontend)
│   ├── index.html
│   ├── medicos.html
│   ├── pacientes.html
│   └── WEB-INF/      # Metadados da aplicação
├── build.xml         # Script de build do Ant
└── nbproject/        # Arquivos de configuração do NetBeans
```

