## O que são branchse?
    As branches são ramificações do código principal, elas são independentes do codigo principal, assim dando a possibilidade de diversas pessoas de trabalhar em diferentes versõe do projeto sem mexer na principal, a não ser que use o merge
    Ex: São como o save de um jogo, que você entra nele para testar builds diferente, e depois de testado é salvo por cima do save original apenas se essa buil der certo

## Comando básicos
    Criar uma branch:
    -git branch nome-branch

    Mudar de branch
    -git checkout nome-branch

    Listar mostrar todas as branchs
    -git branch --list

    Deletar uma branch
    -git branch -d nome-branch

## Usando o merge#
    O merge serve para unir as alterações da ramificação para o codigo principal

    1- Ir para a branch main
    -git checkout main

    2- Executando o merge
    -git merge branch-nome

## Conflitos merge
    Ocorre quando o git não consegue unir automaticamente as alterações

    O que fazer?

    1- Abra o arquivo que está com conflito 
    2- Altere manualmente as alterações que você quer que fique
    3- Adicione o que foi alterado com "git add" e depois use um git commit -m "e a alteração que foi feita"
