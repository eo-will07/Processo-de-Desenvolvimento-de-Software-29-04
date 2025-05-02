# Processo-de-Desenvolvimento-de-Software-29-04

# ------ Incio -------
cd meu_projeto         # entre na pasta do projeto
git init 

# ------ Add os arquivos git --------
git add .                # Add e prepara TODOS os arquivos
# ou
git add src/index.html    # adiciona apenas UM arquivo

# ------ Salvar versão -------
git commit -m "Adiciona página inicial HTML"

# ----- historico -------
git log        # mostra todos os commits


# ------ Controle de mudanças --------
git checkout -b feature/login     # cria branch para o "feature/login"

# ------ Branch Principal e dps o Merge -------
git checkout main            # Volta para o main
git merge feature/login      # mescla as alterações

# ------ Verificando Alterações ----------
git status            # mostra o estado atual
git diff              # compara as mudanças não commitadas

# ------ reverter erro ---------
git checkout -- arquivo_errado.js    # descarta mudanças não commitadas
git log --oneline                    # lista commits copie o hash do commit desejado
git reset --hard [hash]              # volta para a versão especificada

# ------ Fluxo do dia  dia -------
git status                        # Verifica o que mudou
git add .                         # Prepara TODAS as alterações
git commit -m "mensagem clara"    # Ex: "Corrige bug no login"

# ------ trabalho Novo ? faça isto -------
git checkout -b nome_da_feature    # Cria um branch 
# ------ Dps faça as alterações -------
git add .
git commit -m "Implementa feature X"
git checkout main                # Volta pro principal
git merge nome_da_feature        # Une as alterações

# ------ Caso de conflito no Merge -------
# edite o arquivo com o conflito manualmente 
# dps:
git add arquivo_resolvido
git commit -m "Resolve conflito no login"
