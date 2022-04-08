# Novo arquivo repositorio remoto

## Criação de chave SSH
Para a realização da chave ssh foram realizado nos seguintes procedimentos:
* No Git bash insira os comandos:
   * ssh-keygen -t ed25519 -C <email-do-usuario> 
   * eval $(ssh-agent -s)
   * ssh-add id_ed25519 
   * cd <diretorio-onde-foi-instalado-o-ssh>
   * cat id_ed25519
* Copie o codigo apresentado pelo Git bash
* Clique no icone do perfil Git hub localizado na parte superior a direita da tela
* Cique em "settings" => "SSH and GPG keys" => "New SSH key"
* Cole o codigo copiado do Git bash na area KEY
* Clique em "Add SSH key"

## Criação de repositorio remoto
* Clique no icone do perfil Git hub localizado na parte superior a direita da tela
* Clique em "your repositories" => "New" 
* Insira o nome, descrição e tipo de reposiótio (publico ou privado)
   * __Recomenda-se marcar a inicialização do repositorio com o README__
* Por fim clique em "Create repository"

## Clonando repositorio 
* Clique no icone do perfil Git hub localizado na parte superior a direita da tela
* Clique em "your repositories" => "Repositories" 
* Selecione o seu repositório desejado
* Clique no botão "Code"
* Selecione um dos links que será ultilizado para a clonagem (https ou ssh)
   * __Como nova chave SSH foi setada recomenda-se que utlize o link SSH para fazer a clonagem__
* No Git bash insiras os seguintes comandos:
   * cd <diretorio-desejado>
   * git clone <link-github>

## Commitando e subindo repositorio local para o github
Após as alterações e criações dos arquivos do repositorio, abra o Git bash e insira os seguintes comandos
* git add *
* git commit -m "<descrição-da-commit>"
* git push origin main(master)

__Ao abrir o seu repositorio Github você pode observar que as alterações foram feitas com sucesso