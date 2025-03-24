# PAM

--Configuração Inicial
git config --global init.defaultBranch main  
git config --global user.name "[Seu_Usuario]"  
git config --global user.email "[Seu_Email]" 

--Passos com o Repositorio em andamento no GitHub--
Gerando uma pasta com o nome do repositório:
git clone https://github.com/prof-isack/projetos_etec.git
Utilizando o diretório atual como raiz do repositório:
git clone https://github.com/prof-isack/projetos_etec.git .

--Passos com o Repositorio vazio no GitHub--
Acessar o diretório que será raiz do repositório, clicar com o botão direito, abrir GitBash;
ou abrir o GitBash, navegar até o diretorio;
git init 

--Subindo para o repositório--
git add . 
git commit -m "mensagem descritiva referenciando devidamente o que foi feito"
git branch -M main  
git remote add origin https://github.com/prof-isack/projetos_etec.git
git push -u origin main
Obs.: Se origin existente, limpar com "git remote remove origin" 

--Atualizar projeto no respotitório
git status 
git add . 
git commit -m “atualização realizada no projeto em desenvolvimento” 
git push [-u origin main] 

Obs.: Se você não gerou ainda os arquivos "README.md" e ".gitignore", execute no terminal:
echo "título do projeto / descrição mínima" >> README.md
dotnet new gitignore 
