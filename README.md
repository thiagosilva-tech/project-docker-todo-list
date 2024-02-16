## Projeto Docker Todo List

Este projeto envolve a criação de containers Docker para diferentes componentes de uma aplicação de lista de tarefas. Abaixo estão listados os requisitos obrigatórios e o requisito bônus do projeto:

#### Tecnologias Utilizadas

- Docker
- Docker Compose

### Requisitos Obrigatórios

1. **Criação e Execução de Container Alpine**:
   - Crie um container em modo interativo, sem rodá-lo, nomeando-o como `01container` e utilizando a imagem alpine na versão 3.12.
   - Inicie o container `01container`.
   - Liste os containers filtrando pelo nome `01container`.
   - Execute o comando `cat /etc/os-release` no container `01container` sem se acoplar a ele.
   - Remova o container `01container`.

2. **Download e Execução de Imagem Nginx**:
   - Faça o download da imagem nginx com a versão 1.21.3-alpine sem criar ou rodar um container.
   - Rode um novo container com a imagem nginx com a versão 1.21.3-alpine em segundo plano nomeando-o como `02images` e mapeando sua porta padrão de acesso para porta 3000 do sistema hospedeiro.
   - Pare o container `02images` que está em andamento.

3. **Build das Imagens Docker**:
   - Gere uma build a partir do Dockerfile do back-end do todo-app nomeando a imagem para `todobackend`.
   - Gere uma build a partir do Dockerfile do front-end do todo-app nomeando a imagem para `todofrontend`.
   - Gere uma build a partir do Dockerfile dos testes do todo-app nomeando a imagem para `todotests`.

### Requisito Bônus

4. **Orquestração com Docker Compose**:
   - Suba uma orquestração em segundo plano com o docker-compose de forma que backend, frontend e tests consigam se comunicar.

### Conclusão

O projeto Docker Todo List envolve a criação e execução de containers Docker para diferentes componentes de uma aplicação de lista de tarefas. O uso de Docker e Docker Compose facilita a criação, distribuição e execução desses componentes de forma isolada e eficiente.
