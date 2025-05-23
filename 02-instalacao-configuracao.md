# Instalação e Configuração do Git

## Onde baixar e instalar

### Windows

Entre no site oficial do Git: https://git-scm.com/

Baixe o instalador para Windows.

Rode o instalador e siga o passo a passo, pode deixar as opções padrão mesmo.

### macOS

Se tiver o Homebrew instalado, pode usar esse comando no terminal:

```
brew install git
```

Se não, pode baixar direto do site: https://git-scm.com/

### Linux (Debian/Ubuntu)

No terminal, rode esses comandos:

```
sudo apt update  
sudo apt install git
```

## Configurações básicas

Depois de instalar, você precisa configurar seu nome e email, porque o Git usa isso pra saber quem está fazendo as alterações. Use esses comandos:

```
git config --global user.name "Seu Nome"  
git config --global user.email "seuemail@exemplo.com"
```

## Como ver as configurações

Se quiser checar se as configurações estão certas, é só rodar:

```
git config --list
```

## Checar se o Git está instalado

Pra confirmar que o Git está instalado mesmo, digite no terminal:

```
git --version
```

Se aparecer a versão do Git, tá tudo certo.

## Resumo

Pronto! Agora o Git está instalado e configurado no seu computador. Pode começar a usar pra criar seus projetos e trabalhar junto com outras pessoas.

<!-- Linha adicionada para registrar alteração -->
