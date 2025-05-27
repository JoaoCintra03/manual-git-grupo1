## Criar conta no GitHub
Permite que você tenha um perfil no GitHub, onde pode armazenar seus projetos (repositórios), colaborar com outros desenvolvedores e contribuir para projetos open-source.

Acesse github.com, clique em "Sign up" e preencha os dados necessários (e-mail, nome de usuário, senha).



## Repositório Remoto
Um repositório remoto é um projeto hospedado no GitHub (ou em outro serviço como GitLab, Bitbucket). Ele armazena:

Seus arquivos de código (HTML, Python, JavaScript, etc.).

O histórico de alterações (commits).

Documentação (como README.md).

Issues (tarefas/bugs) e Pull Requests (solicitações de mudança).
Como Criar um Repositório Remoto no GitHub?
Passo a Passo
Acesse o GitHub

Entre na sua conta em github.com.

Clique no botão "+" no canto superior direito e selecione "New repository".

Configurações do Repositório

Repository name: Dê um nome ao repositório (ex: meu-projeto).

Description (opcional): Adicione uma breve descrição.

Visibilidade:

Public: Qualquer pessoa pode ver (mas só você edita, a menos que compartilhe).

Private: Somente você e colaboradores autorizados têm acesso.

```
Clique em "Create repository"
```
Pronto! Seu repositório está criado e você verá uma URL como:

https://github.com/seu-usuario/meu-projeto  


Gerenciar o Repositório
Adicionar colaboradores:

Settings > Collaborators > Add people.

Criar branches:

```
git checkout -b nova-feature
git push origin nova-feature
```
Visualizar alterações:

Acesse a aba "Code" no GitHub para ver os arquivos.

Veja o histórico na aba "Commits"

## Clonar um repositório

Baixa uma cópia (cópia local) de um repositório remoto do GitHub para sua máquina.

Quando você quer trabalhar em um projeto existente (seu ou de outra pessoa).

Para contribuir em projetos open-source.

git clone https://github.com/usuario/repositorio.git
Isso criará uma pasta com o nome do repositório no seu computador.


```
git push 
```

(Enviar alterações para o remoto)

Envia ("empurra") suas alterações locais para o repositório remoto (GitHub).

Depois de fazer git add e git commit.

Quando quer atualizar o repositório remoto com suas mudanças.
git push origin main  # (ou "master" em repositórios antigos)
origin = nome padrão do repositório remoto.

main = branch para onde você está enviando.

## git pull Atualizar seu repositório local

Puxa ("puxa") as alterações mais recentes do repositório remoto para sua máquina local.

Antes de começar a trabalhar em um projeto compartilhado.

Se alguém fez alterações no repositório remoto e você quer atualizar sua cópia.

```
git pull origin main
```

Isso faz um git fetch (baixa as alterações) + git merge (mescla na sua branch atual).

Sempre faça git pull antes de git push para evitar conflitos.
Use git status para verificar o estado do seu repositório.
Se der conflito, resolva manualmente e depois faça git add + git commit.

Um Pull Request (ou "Solicitação de Atualização") é um pedido para que as alterações feitas em uma branch sejam incorporadas (mergeadas) em outra branch (geralmente a main ou master).

Quando você quer contribuir para um projeto open-source.

Em equipes de desenvolvimento, para revisar mudanças antes de mesclá-las.

Para discutir melhorias ou correções antes de integrar o código.



## Como Criar um Pull Request
Faça um Fork (se for um projeto de terceiros)

No GitHub, clique em "Fork" no canto superior direito do repositório original.

Isso cria uma cópia do projeto na sua conta.

Clone o repositório para sua máquina

git clone https://github.com/seu-usuario/repositorio.git

```
cd repositorio
```

Crie uma branch para suas alterações

```
git checkout -b minha-feature
```
Faça as alterações e envie para o GitHub

```
git add .
git commit -m "Adiciona nova funcionalidade"
git push origin minha-feature
```
Abra o Pull Request no GitHub

Vá até o repositório original no GitHub.

Clique em "Pull requests" > "New pull request".

Selecione sua branch (minha-feature) e a branch de destino (main).

Descreva suas mudanças e clique em "Create pull request".

## Revisão de Código (Code Review)

Revisores podem comentar trechos do código para sugerir melhorias.

Aprovação (Approve)

Um revisor pode aprovar o PR se estiver tudo correto.
 Solicitação de Alterações (Request Changes)

Se algo precisa ser corrigido, o revisor pode bloquear o merge até que as mudanças sejam feitas.

Muitos projetos rodam testes automatizados (GitHub Actions, Travis CI) para verificar se o PR não quebra nada

```
.git checkout main
git pull origin main
git checkout minha-feature
git merge main
```