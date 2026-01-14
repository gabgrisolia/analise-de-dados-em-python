# Comandos Git para Subir no GitHub

## Se o repositório ainda não foi inicializado:

```bash
# 1. Inicializar o repositório Git (se ainda não foi feito)
git init

# 2. Adicionar o remote do GitHub (substitua pela URL do seu repositório)
git remote add origin https://github.com/gabgrisolia/seu-repositorio.git
```

## Comandos para adicionar e fazer commit da aula2:

```bash
# 1. Adicionar todos os arquivos da pasta aula2
git add aula2/

# 2. Verificar o que será commitado
git status

# 3. Fazer o commit
git commit -m "Adiciona projeto de análise de cancelamento de clientes - aula2"

# 4. Fazer push para o GitHub
git push origin main
```

## Se você já tem um repositório configurado:

```bash
# Adicionar apenas os arquivos da aula2
git add aula2/README.md aula2/requirements.txt aula2/inicial.ipynb aula2/cancelamentos.csv

# Ou adicionar toda a pasta
git add aula2/

# Fazer commit
git commit -m "Adiciona projeto de análise de cancelamento de clientes - aula2"

# Fazer push
git push origin main
```

## Comandos alternativos (se estiver em outra branch):

```bash
# Verificar em qual branch você está
git branch

# Se estiver em outra branch (ex: master), use:
git push origin master

# Ou mude para main:
git checkout main
git push origin main
```
