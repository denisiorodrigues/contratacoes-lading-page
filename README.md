# Contrataçõoes

Uma empresa de TI quer desenvolver uma página destinada a novas contratações e contratou você para desenvolvê-la.

Para isso, te enviaram um layout no Figma. E a partir desse protótipo, o objetivo é transformá-lo em código e dar vida real ao projeto.

## Índice

* [Visão Geral](#visão-geral)
* [Funcionalidades](#funcionalidades)
* [Tecnologias Utilizadas](#tecnologias-utilizadas)
* [Layout](#layout)
* [Como Usar](#como-usar)
* [Dica](#dica)

---

## Visão Geral

Este é um projeto de uma aplicação web que permite qualquer pessoa possa acessar e visualizar as vagas disponibilizadas na página.

## Funcionalidades

Abaixo as principais funcionalidades ou características do projeto.

* Visualizar as informções da empresa;
* Visualizar as vagas de emprego;
* Permitir informar o e-mail para receber as oportunidades.

## Tecnologias Utilizadas

Abaixo as principais tecnologias que está sendo utilizada para construir este projeto.

* **Linguagens**: [HTML, CSS] (Mesmo nao sendo linguagem e sim marcação de texto)
* **Ferramentas**: [Git, Figma]
* **Link do Repositório**: [https://github.com/denisiorodrigues/contratacoes-lading-page.git](https://github.com/denisiorodrigues/contratacoes-lading-page.git)

## Layout

### Desktop
![Layout da Aplicação](./docs/layout_main.png)


[Figma do projeto](https://www.figma.com/design/mm3MLozvUDGhDRTxSLlGL5/7daysOfCode-HTML-CSS?node-id=0-1&p=f&t=mHlUzPcnfhwNM5Ly-0)

## Como Usar

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/denisiorodrigues/contratacoes-lading-page.git
    ```
2.  **Navegue até a pasta do projeto:**
    ```bash
    cd apperia
    ```
3. **Execute a aplicação:**

    Instalar a extenção **Live Server** no VS Code ou clicar no arquivo index.html 

## Dica

Abaxi problemas relatados e corrigidos no processo

### Erro de token
Se o erro for como o debaixo, é porque as operações do git não suporta mais autenticação por senha. (isso é o que eu acho)
Se você tem o uma chave SSH cadastrada, nao precisa fazer login, o problema é que o token de acesso está expirado. Uma das soluções para resolver esse problema é gerar o token no github, se esse e o servidor do repositório que está utilizando, esse é o meu caso.   

```bash
    Username for 'https://github.com': denisiorodrigues
    Password for 'https://denisiorodrigues@github.com': 
    remote: Invalid username or token. Password authentication is not supported for Git operations.
    fatal: Authentication failed for 'https://github.com/denisiorodrigues/contratacoes-lading-page.git/'
```

Para Gerar o token siga o passo a passo a seguir neste [link da geeksforgeeks](https://www.geeksforgeeks.org/git/how-to-generate-personal-access-token-in-github/).

Depois do token gerado, precisamos configurar no repositório, seguindo esse passo a passo.

1.  **Copie o token gerado, como por exemplo:**
    ```bash
    ghp_Spw90V7Sumuwq8Jxui8sGgq12U1Pga26vVvkL
    ```
2.  **Execute o comando:**
    ```bash
    git remote set-url origin https://<cole-o-token-gerado-aqui>@github.com/<seu-usuário>/<seu-repositorio>.git
    ```