Git Init
O comando git init é o primeiro passo para começar a usar o Git em um projeto. Ele inicializa um novo repositório Git vazio ou reinicializa um existente no diretório atual.

Exemplo Prático: Imagine que você tem uma pasta chamada meu-manual. Para transformá-la em um 

ˋˋˋ
repositório Git:
cd meu-manual
git init
Inicialized empty Git repository in /caminho/para/meu-manual/.git/
ˋˋˋ


Git Add
O comando git add é usado para adicionar alterações de um arquivo para a "staging area" (área de preparação). Isso significa que você está informando ao Git que essas mudanças específicas devem ser incluídas no próximo commit

Exemplo Prático: Para adicionar o arquivo 03-comandos-basicos.md à área de preparação:
git add arquivo.md

ˋˋˋ
Git Status
Use git status para ver o estado atual do seu repositório Git. Ele mostra quais arquivos foram modificados, quais estão prontos para serem commitados (staged), e quais não estão sendo rastreados pelo Git
ˋˋˋ

Exemplo Prático: Após criar o arquivo arquivo.md na pasta meu-manual


ˋˋˋ
git status"
On branch main
No commits yet
Changes to be committed:
(use "git rm --cached <file>..." to unstage)
new file:   arquivo.md"
ˋˋˋ

Git Commit
Após adicionar suas alterações à staging area, git commit as registra permanentemente no histórico do seu repositório. Cada commit deve ter uma mensagem descritiva que explique as mudanças feitas. É uma boa prática usar mensagens semânticas (ex: feat:, fix:, docs:).

Exemplo Prático: Para salvar as alterações do arquivo.md:

ˋˋˋ
git commit -m "feat: Adiciona módulo de comandos básicos ao manual"
Saída esperada:
[main (root-commit) e9f8g7h] feat: Adiciona módulo de comandos básicos ao manual
1 file changed, 50 insertions(+)
create mode 100644 arquivo.md
ˋˋˋ


Git log
git log exibe o histórico de commits do seu repositório. Ele mostra informações como o hash do commit (identificador único), o autor, a data e a mensagem de cada commit.

Exemplo Prático: Para ver o histórico após seu commit:

ˋˋˋ
git log
commit e9f8g7h6i5j4k3l2m1n0o9p8q7r6s5t4u3v2w1x0 (HEAD -> main)
Author: Seu Nome <seu.email@example.com>
Date:   Fri May 31 14:30:00 2025 -0300

feat: Adiciona módulo de comandos básicos ao manual
ˋˋˋ
