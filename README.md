## Curso Git 

#### Comandos do git

* git help - Mostra os comandos do git e uma breve descrição do seu funcionamento

* git help [comando] - Mostra as informações de um comando específico 

* git init - Cria um repisotorio Git no diretorio autual, todas as configurações do repositório ficam na pasta oculta .git

* git add [arquivo] - adiciona um arquivo do repositório ao controle de versão (git add - adiciona todos os arquivos do diretório ao Git)

* git commit -m "Mensagem" - Comitta as mudanças adicionadas (Comittar é gerar a mudança no repositório) exibindo a mensagem passada entre as aspas (a mensagem é obrigatória)

* git config - Modifica ou define as configurações do diretório atual (Ex: conta relacionada ao diretório)

* git config --global - Realiza as modificações na configuração para todos os repositórios

* git status - Mostra o status do repositório, caso o repositirio tenha sido alterado ou se ha commits a serem realizados

* git log - Mostra o histórico de commits que foram feitos

* git remote add origin [endereço do git remto] - adiciona o repositorio para um Git remoto (ex: GitHub, GitLab)

* git push -u origin master - Envia os commits feitos no repositorio atual para o remote no branch master (branch principal do repositorio remoto) - Esse comando so precisa ser usado na primeira vez que for feito um push

* git push - comando usado para enviar os commits para o repositorio remoto assiciado a um repositorio local (Esse comando é usado a partir da sugunda vez que um push for feito) 

* git rm [arquivo] - Remove um arquivo do repositorio

* git diff - Mostra a diferença entre commits e braches (para mostrar as alterações des de o ultimo commit deve-se adicionar HEAD~1)

* git clone - Baixa um repositorio remoto(ja vem configurado)

* git pull - Baixa as alterações do repositorio remoto (Mantém o repositorio sincronizado com os ultimos commits de uma branch)

* git checkout [commit] [file] - Permite ver como um arquivo ou todo o repositorio estava em um determinado commit (Para retornar para o estado atual do repositorio basta dar git checkout master)

* git checkout -- [arquivo] - Desfaz as mudanças que não foram adicionadas em um arquivo (git checout -- * - desfaz as mudanças que não foram adicionadas em todos os arquivos)

* git checkout HEAD -- [arquivo] - Desfaz alterações que ja foram adicionados em um determinado arquivo

* git rever [commit] - Irá criar um novo commit que desfaz as alterações do commit especificado (Útil para desfazer um commit antigo)

* git reset [commit] - Reseta o repositório para um determinado commit

* git reset --hard [commit] - Resetar e remover todas as alterações (Não usar seja estiver publicado)

* git branch  - mostra as branches do repositório

* git branch [nova_branch] - cria uma nova branch

* git branch -d [branch] - Exclui uma branch

* git checkout [branch] - Muda para a branch (O repositorio passa a ter os commits que a branch possuir e novos commits serão adicionados a ela)

* git merge [branch] - Aplica os commits de uma branch na branch atual (Encontra um commit comum (base) entre as branches e aplica todos os commits que a branch atual não possui, caso existam commits na branch atual que não estejam na outra é criado um commit de merge)


#### Estados dos arquivos

* untracked - Não monitorado (quando o arquivo é criado)

* modified - Modificado (quando o arquivo é modificado em relação ao ultimo commit)

* staged - Preparado (quando o aquivo é adicionado e está pronto para ser commitado)

* commited - Consolidado (Quando o arquivo tem o seu estado registrado no repoistório)

#### Conflitos

* Conflitos podem acontecer ao unirmos alterações

* Acontecem quando versões diferentes possuem as mesmas linhas nos mesmos arquivos editadas de formas diferentes

* O Git identifica os conflitos e fica aguardando a solução deles

* Ao resolver os conflitos deve ser feito um commit

#### Branching

* São ramificações do repositório - desenvolvimentos diferentes de um mesmo código

* É uma lista de commits

* Muito util para trabalhos colabrativos

* Branches de desenvolvimento facilitam o controle

* A Branch master é a padrão


