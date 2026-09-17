# 💬 Chat Laravel Pusher

Sistema de chat desenvolvido com **Laravel, Chatify e Pusher**, criado como atividade acadêmica para explorar o desenvolvimento de aplicações web com autenticação de usuários, comunicação em tempo real e integração com banco de dados.

O projeto permite que usuários se cadastrem, realizem login e interajam por meio de conversas, enviando mensagens para outros usuários cadastrados na plataforma.

## **🚀 Tecnologias Utilizadas**

* **Laravel:** Framework PHP utilizado para a estruturação e desenvolvimento da aplicação web.
* **Laravel Breeze:** Responsável pelo sistema de autenticação, incluindo cadastro, login e gerenciamento de sessão dos usuários.
* **Chatify:** Pacote utilizado para implementar o sistema de conversas e envio de mensagens.
* **Pusher:** Serviço utilizado para auxiliar na comunicação em tempo real entre os usuários.
* **MySQL/MariaDB:** Banco de dados responsável pelo armazenamento das informações da aplicação.
* **Vite:** Ferramenta utilizada para gerenciar e compilar os recursos front-end.
* **Composer:** Gerenciador de dependências do PHP.
* **NPM:** Gerenciador de pacotes utilizado para as dependências do front-end.

## **📌 Objetivo do Projeto**

O principal objetivo do projeto é desenvolver um sistema de chat utilizando o framework Laravel e tecnologias relacionadas à comunicação em tempo real.

A aplicação foi desenvolvida para colocar em prática conceitos como:

* **Autenticação de usuários.**
* **Rotas e middlewares do Laravel.**
* **Integração com banco de dados.**
* **Utilização de pacotes externos.**
* **Comunicação em tempo real.**
* **Armazenamento e recuperação de mensagens.**
* **Desenvolvimento de interfaces web.**

## **⚙️ Funcionalidades**

* **Cadastro de usuários:** Permite criar uma conta com nome, e-mail e senha.
* **Login:** Usuários cadastrados podem acessar a plataforma por meio de suas credenciais.
* **Dashboard personalizado:** Após o login, o usuário é direcionado para uma área principal personalizada.
* **Sistema de conversas:** Permite acessar e iniciar conversas com outros usuários.
* **Envio de mensagens:** Usuários podem enviar mensagens dentro de uma conversa.
* **Armazenamento de mensagens:** As mensagens são registradas no banco de dados por meio do sistema de chat.
* **Autenticação e proteção de rotas:** As áreas restritas da aplicação exigem que o usuário esteja autenticado.

## **🔄 Como o Projeto Funciona**

O funcionamento da aplicação ocorre por meio de um fluxo de autenticação e comunicação entre usuários.

Primeiramente, o usuário realiza seu cadastro na plataforma. As informações da conta são armazenadas no banco de dados, permitindo que ele utilize suas credenciais para realizar o login posteriormente.

Após a autenticação, o usuário é direcionado para o **Dashboard**, que funciona como a área principal do sistema. Nessa tela, é possível acessar o sistema de chat por meio do botão disponibilizado na interface.

Dentro do Chatify, o usuário pode visualizar as conversas disponíveis, selecionar outro usuário e enviar mensagens. As informações das conversas e das mensagens são armazenadas no banco de dados, enquanto o Pusher auxilia na comunicação e atualização em tempo real, conforme a configuração da aplicação.

## **🗄️ Banco de Dados**

O projeto utiliza **MySQL/MariaDB** para armazenar os dados da aplicação.

O banco de dados utilizado durante o desenvolvimento é:

```text
chatweb3ams
```

Entre as informações armazenadas estão:

* **Dados dos usuários cadastrados.**
* **Informações relacionadas às conversas.**
* **Mensagens enviadas entre os usuários.**
* **Dados necessários para o funcionamento do sistema de autenticação e chat.**

As tabelas são criadas e atualizadas por meio das migrations do Laravel e dos pacotes instalados no projeto.

## **💬 Comunicação em Tempo Real**

O projeto utiliza o **Pusher Channels** como parte da implementação de comunicação em tempo real.

O Pusher permite que eventos relacionados ao sistema sejam transmitidos entre o servidor e os clientes conectados, contribuindo para a atualização das conversas sem a necessidade de atualizar manualmente a página em determinadas situações.

O Chatify é responsável pela estrutura do sistema de mensagens, enquanto o Laravel gerencia a lógica da aplicação e a integração com o banco de dados.

## **🔐 Autenticação e Segurança**

A autenticação da aplicação é implementada utilizando o **Laravel Breeze**, que fornece uma estrutura inicial para cadastro, login e gerenciamento de usuários.

As rotas protegidas utilizam o middleware `auth`, garantindo que determinadas páginas, como o Dashboard e o sistema de chat, sejam acessadas somente por usuários autenticados.

As senhas dos usuários são armazenadas utilizando hash, evitando que sejam salvas diretamente em texto puro no banco de dados.

## **📥 Como Executar o Projeto**

### **1. Clonar o repositório**

```bash
git clone URL_DO_REPOSITORIO
```

### **2. Acessar a pasta do projeto**

```bash
cd chatLaravelPusher
```

### **3. Instalar as dependências do PHP**

```bash
composer install
```

### **4. Instalar as dependências do front-end**

```bash
npm install
```

### **5. Configurar o arquivo `.env`**

Crie ou configure o arquivo `.env` com as informações do banco de dados e as credenciais do Pusher.

### **6. Executar as migrations**

```bash
php artisan migrate
```

### **7. Iniciar o Vite**

```bash
npm run dev
```

### **8. Iniciar o servidor Laravel**

Em outro terminal, execute:

```bash
php artisan serve
```

Após iniciar os serviços, acesse a aplicação pelo endereço disponibilizado pelo Laravel, normalmente:

```text
http://127.0.0.1:8000
```

## **📚 Aprendizados**

O desenvolvimento deste projeto proporcionou a prática de conceitos relacionados ao desenvolvimento web utilizando Laravel, incluindo a criação de sistemas de autenticação, integração com banco de dados, utilização de pacotes externos e implementação de funcionalidades de comunicação entre usuários.

Além disso, o projeto contribuiu para a compreensão do funcionamento de aplicações que utilizam comunicação em tempo real e persistência de dados.

## **👨‍💻 Desenvolvedor**

Desenvolvido por **Renan Pereira** como atividade acadêmica de desenvolvimento web e implementação de um sistema de chat utilizando Laravel, Chatify e Pusher.
