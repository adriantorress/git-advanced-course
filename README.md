# PHOTO PORTFOLIO

> A simple project to learn day by day git

Big Picture by HTML5 UP

html5up.net | @ajlkn

Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)

## GOOD HABITS - MERGE / REBASE

> Está atualizando sua branch pegando as coisas do master?

USE REBASE (PULL --REBASE)

> Terminou sua feature no branch e quer jogar para o master?

USE MERGE

## VSCODE TIPS

> Ctrl + Shift + P (Algumas coisas para o git no vscode: git history log, remote, branch... com isso, e mais o Controle do Código-Fonte (Ctrl + Shift + G), da pra utilizar o git diretamente no vscode, fora da linha de comando)

> Git blame: extensão que mostra o último commit de cada linha e o autor que o fez



## GIT COMMANDS
**git branch --set-upstream-to=origin/<branch> <branch-atual>**

> Seta uma branch para a qual sua branch atual vai ficar trackeando mudanças, como se fosse a branch do qual ela foi originada

**git commit --amend**

> Permite editar um commit já feito antes de subir para o Github

**git cherry-pick (*chave*)**

> Pega um commit especifico de uma outra branch para a atual sem precisar fazer merge ou rebase

**git add -p**

> Permite escolher o que, dentro de um arquivo, colocar ou não em staged 

**git rebase -i HEAD~(número de commits a serem alterados)**

> Com o git rebase da para fazer também junções de commits, com o **squash**, e alterar também a mensagem após a junção 

**git commit --fixup (*chave*)**

> Fixa um erro de algum commit anterior

**git rebase -i --autosquash (*chave*)**

> Junta todos os commits que estão fixup, com o autosquash, com o commit subsequente a chave passada

**git merge --continue**

> Continua o merge após resolver um conflito

**git config --global help.autocorrect 1**

> Ajuda a corrigir pequenas falhas de digitação de algum comando

**git archive (master // branch) --format=(zip//formato) --output=(master.zip // Nome do arquivo)**

> Permite zipar as pastas e arquivos de uma branch

**git log --pretty=oneline --graph -all**

> Customiza a visualização do log: 
>--pretty=online, mostra cada commit por linha. 
>--graph, mostra de forma gráfica uma linha do tempo com o histórico de commits. 
>--all, mostra todas as branchs no log e não só a atual.

**git log --since='Month dd yyyy'**

> Mostra todos os commits desde certa data

**git log --until='Month dd yyyy'**

> Mostra todos os commits até certa data. Pode ser usado junto com o since

**git log --author=(*'author_name'*)**

> Mostra todos os commits feitos por determinado autor.

**git shortlog -sn**

> Mostra todos os commits de forma resumida. com o -sn mostra somente o autor e o numero de commits

**git log (*quantidade de commits a ser mostrados*)**

> Mostra a quantidade de commits desejada a partir do ultimo.

**git reflog**

> Mostra os logs de uma forma mais completa, pois diferente do git log que mostra apenas os commits, o git reflog trabalha em cima das referências, ou seja, vai mostrar todo tipo de alteração feita em cada branch, conseguindo pegar até mesmo mudanças anteriores ao reset --hard

**git push origin --delete <branch>**
> Comando para deletar uma branch remota 

## GIT TIPS

> Nunca altere o histórico no master, caso haja algum erro em algum dado commit, use o revert - que gera um novo commit com a reversão do commit desejado, mas não mexe no histórico

> Ou seja: git revert serve para o master e o git reset é bom para outras branches

## GITHUB LEARNING

### USUÁRIOS

> No github não existem somente pessoas enquanto usuários, mas também organizações. Essas organizações possuem repositórios e também possui pessoas. 

### NOTIFICAÇÕES

> Na aba de NOTIFICAÇÕES da para habilitar as preferências.

### STAR

> O STAR é uma forma de apoiar o projeto / dizer que gostou, curtiu...

### FORK

> O FORK faz uma cópia do estado atual de um projeto para o seu portfólio, não sofrendo com possíveis modificações no projeto original. O FORK também é útil para fazer contribuições para um projeto, você pode copiá-lo para seu repositório, fazer alterações e submetê-las para o proprietário.

### ISSUES

> As ISSUES servem basicamente para relatar algum problema / alguma melhoria que possa ser feita. 

> Foram criadas para criar discussões sobre o projeto. 

> Toda issue possui um ID.

> A issue pode estar aberta (ainda não foi concluída) ou fechada (já concluída). 

> Ao criar a issue, você pode determinar uma pessoa para resolver aquela tarefa através da aba assignes dentro da issue. 

> Da para criar labels para categorizar a issue.

> É possível determinar de qual projeto é aquela issue.

> Da para agrupar issues pelo Milestone - determinando assim o estado atual do projeto, se é uma versão beta ou alfa, se já está pronto, etc.

> Da para ativar as notificações de atualizações de determinada issue e também ver os participantes dela. 

> Muitas empresas costumam trabalhar com issues para definir o workflow do projeto, coisas que precisam ser melhoradas/modificadas através dessas issues. 

> É possível criar issues a partir de trechos do código, customizar a issue (adicionando check-boxs e outros tipos de customização) e também da para inserir screenshots do task de determinada issue.

> É possível também criar um template para as issues, basta criar uma pasta ".github", adicionar o arquivo issue_template.md e descrever como você deseja que seja criada as issues pro seu projeto. E quando você ou algum contribuidor do projeto for criar uma nova issue, aparecerá o formato que você definiu para que baseiem-se nele.

> É possível referenciar issues umas nas outras (colocando um comentário na issue que irá referenciar com um # + o numero da issue a ser referenciada).

> As issues podem ser fechadas e reabertas nelas mesmo, mas também podem ser fechadas através das mensagens do commit, passando o comando - Closes #numero_da_issue na mensagem a issue será fechada no repositório.

### PULL REQUESTS

> PULL REQUESTS: submissão de um código para melhoria de algum detalhe.

> Branch ou commit separado onde pretende-se liga-lo ao branch principal.

> Pedir para a correção ou mudança seja aceita no branch principal, que geralmente, mas não necessariamente, é o master.

> Ou seja, manda-se o código e faz o pedido para ver se ele é aceito ou não e se esse é mergeado ou não no branch desejado.

> Ao subir a branch para o repositório, vai aparecer a sugestão de Pull Request.

> O Pull Request (PR) pode ser customizado assim como as Issues - colocando labels e todas as outras opções.

> Da para criar mini-tabelas com screenshots do antes e depois.

> Assim como as issues também da para criar um template personalizado do PR, seguindo os mesmos passos: ir na pasta .github, adicionar um arquivo e nomeando-o de pull_request_template.md e fazer o template da sua maneira. Há também um repositório da devspace que contém muitos templates pré-montados - chamado awesome-github-templates.

### PROJECTS

> PROJECTS: da para separar bem o desenvolvimento do projeto em To Do, In Progress, e Done, um workflow. Da para organizar o repositório com cards.

### WIKI

> WIKI: um mapeamento do projeto, da para colocar uma documentação melhorada, planos para o futuro...

### INSIGHTS

> INSIGHTS: um overview do projeto -> Merged / Proposed Pull Requests, Closed / New Issues e mais detalhes do projeto

### SETTINGS

> SETTINGS: Configurações necessárias do repositório

#### BRANCH PROTECTION RULES

> É possível em settings proteger a branch principal do projeto, basta ir em branches, em "Branch protection rules" clicar em "Add rule" e em "Branch name pattern" digitar "main" (ou o nome da sua branch principal). Basta selecionar as opções de proteção que deseja habilitar, por exemplo: você pode exigir que todos os pushs para a branch principal passem em verificações de status antes de serem mesclados. No final é só salvar.

> Nesse projeto foi aplicado essas regras para a branch master:

> "Require a pull request before merging" (Requerer um pull request antes do merge): Todos os commits devem ser feitos em um branch não protegida e submetidos via pull request antes que possam ser mesclados na branch principal.

> "Require approvals" (Requerer aprovações): Os pull requests requerem um número de aprovações e não podem ter solicitações de alteração antes de serem mesclados.

> "Dismiss stale pull request approvals when new commits are pushed" (Rejeitar aprovações de pull request obsoletas quando novos commits são feitos): Novos commits revisáveis descartarão as aprovações de pull request.

> "Require status checks to pass before merging" (Requerer que os checks de status sejam aprovados antes do merge): Escolha quais checks de status devem ser aprovados antes que os branches possam ser mesclados na branch principal. Os commits devem primeiro ser enviados a outro branch e, em seguida, mesclados ou enviados diretamente para o branch principal após a aprovação dos checks de status.

> "Require branches to be up to date before merging" (Requerer que os branches estejam atualizados antes do merge): Os branches devem estar atualizados com o branch principal antes do merge.

### PROCESS UNTIL AND AFTER CODE REVIEW

> Cria-se um branch separado

> Faz as devidas mudanças

> Manda isso como Pull Request

> Recebe os comentários

> Trabalha-se em cima desses comentários e faz as correções

> Uma vez feita as correções e recebendo o approval é só fazer o merge para o master

> Há 3 tipos de merge que podem ser feitos no PR, apenas o merge com todos os commits feitos no PR, um squash e merge, que vai juntar todos os commits em um só e fazer o merge, e o rebase e merge, que vai colocar os commits para o topo do histórico e fazer o merge.

> Após finalizar o merge, é bom deletar o branch que foi feito o merge, no caso desse projeto, o branch reorder-sections. Como ele não vai será mais utilizado, é bom deletar para manter o git e o github organizado.



## WORKFLOW LEARNING

> Fluxo de trabalho

> Sequência de passos necessários para automatizar processos, de acordo com um conjunto de regras definidas, permitindo que possam ser transmitidos de uma pessoa para outra

> Passo a passo das tarefas dentro do git ou qualquer outra coisa

> No git: Desde o momento de salvar o arquivo, criar um commit, enviar esse commit pro github, pedir um pull request, fazer o code review e até fazer o merge para o master para ter essas mudanças na aplicação. Pequenos passos feitos desde o desenvolvimento até o envio para a produção 

### GIT WORKFLOWS

#### CENTRALIZED WORKFLOW

> Centralized Workflow: Branch único (Master); 

> Fácil para transição de quem vem do SVN;

> Funciona melhor com equipes bem pequenas - de 3 a 4 pessoas;

> Exemplo do workflow: pessoa 1 desenvolve uma feature e sobe para o master; pessoa 2 também desenvolveu uma feature e tentou subir para o master, vai dar conflito pois o repositório local dela não está atualizado com o repositório remoto, a pessoa 2 terá que fazer um pull rebase para trazer as mudanças que estão no repositório remoto e colocar as suas mudanças locais acima das mudanças trazidas no histórico, assim ela conseguirá subir sua feature para o github com o push.

#### FEATURE BRANCH WORKFLOW

> Feature Branch Workflow: um dos mais famosos que existem;

> Amplamente utilizado;

> Muito simples de trabalhar;

> Um branch para cada feature: toda vez que for criar uma nova feature, cria-se um novo branch separado baseado no master, trabalha-se na feature desejado e quando finaliza-la faz-se um pull request para o master, passa pelo code review e se estiver tudo certo faz-se o merge;

> Evita muitos conflitos e permite trabalhos em paralelo: funciona com várias pessoas trabalhando no repositório, e como as pessoas vão estar trabalhando nos seus próprios branches, a única preocupação a se ter é manter seu branch atualizado com o master;

> Funciona bem com equipes maiores;

> Cada vez que uma feature entra no master é bem identificável pois sempre será um merge de um branch de feature, facilitando a visualização do histórico.

> Ao final sempre fazer o squash dos commits que não são importantes.

> Foi utilizado nesse projeto :);


#### GITFLOW WORKFLOW

> Gitflow Workflow: Conjunto de extensões para o git que provê operações de alto-nível para repositórios usando o modelo de branches do Vincent Driessen.

> Para aprender mais sobre o gitflow, instalação e fluxo: http://danielkummer.github.io/git-flow-cheatsheet/

> Sobre o fluxo do gitflow: Vai se criar uma branch develop, na branch master vai se startar o git flow com o init e definir as funções das branches. Ao criar uma nova feature e publicar ela no github, voce faz o pull request com a base na branch develop e finaliza a feature pelo terminal, a feature será mergeada na branch develop e será excluída local e remotamente. 

> Você pode criar uma nova release para jogar o código de develop para a branch master: Cria e finaliza a release, escreve uma mensagem para a tag da release, o git fará um merge da release na branch master e develop e apagará o branch da release, e logo após você deve subir a tag para o repositório remoto através da branch master.

> O mesmo sobre releases vale para os hotfixes.

#### GITFLOW COMMANDS

**git flow init** 

> Comando para iniciar o git flow

**git flow feature start <branch name>**

> Comando para iniciar uma nova feature

**git flow feature publish <branch name>**

> Comando para publicar uma nova feature no github 

**git flow feature finish <branch name>**

> Comando para finalizar uma feature

**git flow release start <release name>**

> Cria uma nova release

**git flow release finish <release name>**

> Finaliza uma release


**git flow hotfix start <hotfix name>**

> Inicia um novo hotfix

**git flow hotfix finish fix-anchor**

> Finaliza um hotfix


