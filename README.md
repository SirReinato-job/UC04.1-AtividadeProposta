# Atividade de Versionamento - Git e GitHub

Este projeto foi desenvolvido como parte de uma atividade prática para o curso Full Stack, com o objetivo de aplicar conceitos de versionamento utilizando Git e GitHub. A atividade foca em preservar o histórico de alterações, conciliar mudanças e gerenciar versões em um repositório.

## Objetivo

Aplicar o versionamento de código com Git, manipulando branches e resolvendo conflitos de merge entre diferentes alterações no código.

## Passo a Passo Realizado

1. **Instalação do Git**  
   - Acessado o site [https://git-scm.com/download/win](https://git-scm.com/download/win).
   - Feito o download e instalação da ferramenta Git.
   
2. **Configuração Inicial**  
   - Criado o usuário local com o comando:
     ```bash
     git config --global user.name "Seu Nome"
     ```
   - Definido o e-mail com:
     ```bash
     git config --global user.email "seu.email@exemplo.com"
     ```

3. **Criação de Repositório Local e Remoto**  
   - Criado um repositório local Git com:
     ```bash
     git init
     ```
   - Criado um arquivo `index.txt` no repositório local.
   - Feito o cadastro no GitHub e criado um repositório remoto.
   - Adicionado o repositório remoto com:
     ```bash
     git remote add origin <URL_DO_REPOSITORIO>
     ```

4. **Principais Comandos Utilizados**  
   - `git status` - Verificar o status das alterações no repositório.
   - `git add` - Adicionar as mudanças para o próximo commit.
   - `git commit` - Criar um commit com as alterações.
   - `git push` - Publicar as alterações no repositório remoto.
   - `git checkout` - Trocar de branch.
   - `git merge` - Unir as alterações de uma branch a outra.
   - `git pull` - Puxar as alterações do repositório remoto para o local.

5. **Conteúdo do Arquivo `index.txt` Inicial**
   ```html
   <HTML>
   <HEAD><TITLE>ATIVIDADE DE VERSIONAMENTO</TITLE></HEAD>
   <BODY>
      <H1> TÍTULO1 </H1>
   </BODY>
   </HTML> ```
  
6. **Criação de Branch e Modificação**  
   - Criada uma nova branch chamada `feature1` e publicada a mesma versão do arquivo `index.txt` na nova branch.
   - Realizadas alterações na linha `<H1>` em cada branch:
     - Na branch `main`, o conteúdo do arquivo foi alterado para:
       ```html
       <HTML>
       <HEAD><TITLE>ATIVIDADE DE VERSIONAMENTO</TITLE></HEAD>
       <BODY>
          <H1> VERSIONAMENTO </H1>
       </BODY>
       </HTML>
       ```
     - Na branch `feature1`, o conteúdo do arquivo foi alterado para:
       ```html
       <HTML>
       <HEAD><TITLE>ATIVIDADE DE VERSIONAMENTO</TITLE></HEAD>
       <BODY>
          <H1> GIT </H1>
       </BODY>
       </HTML>
       ```

7. **Merge e Resolução de Conflitos**  
   - Realizado o merge da branch `feature1` na branch `main` com o comando:
     ```bash
     git merge feature1
     ```
   - Durante o merge, foi detectado um conflito devido às alterações divergentes na linha `<H1>`.
   - Resolvido o conflito editando o arquivo para consolidar as mudanças conforme o objetivo do projeto, e em seguida finalizado o merge.

8. **Publicação no Repositório Remoto**  
   - Após resolver o conflito, as mudanças foram confirmadas e o código foi publicado no repositório remoto com os comandos:
     ```bash
     git add index.txt
     git commit -m "Resolução de conflito de merge entre main e feature1"
     git push origin main
     ```

## Ferramentas Utilizadas

- **Git** - Para controle de versão local.
- **GitHub** - Para repositório remoto e colaboração.

## Conclusão

Este exercício permitiu aplicar comandos básicos e intermediários do Git, como manipulação de branches, resolução de conflitos e publicação de código. A prática reforçou a importância do controle de versão, tornando o desenvolvimento colaborativo mais seguro e organizado.

