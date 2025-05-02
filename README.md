# Processo-de-Desenvolvimento-de-Software-29-04

# Repositorio Git
cd meu_projeto  # entra na pasta do projeto
git init        # inicia o versionamento

# Add os arquivos Git
git add .       # prepara TODOS os arquivos para commit
# ou
git add src/index.html  # adiciona apenas UM arquivo

# Salvar Versão
git commit -m "Adiciona página inicial HTML"  # mensagem clara!

# Verificar historico
git log  # mostra todos os commits


# Controle de mudanças
git checkout -b feature/login  # cria branch "feature/login"

# Branch Principal
git checkout main

# Branch na versão principal
git merge feature/login  # une as alterações ao branch main
