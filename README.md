# Photo portfolio

> A simple project to learn advanced git

Big Picture by HTML5 UP

html5up.net | @ajlkn

Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)

## Boas Práticas - Merge / Rebase

> Está atualizando sua branch pegando as coisas do master?

USE REBASE (PULL --REBASE)

> Terminou sua feature no branch e quer jogar para o master?

USE MERGE

## VSCode tips

> Ctrl + Shift + P (Algumas coisas para o git no vscode: git history log, remote, branch... com isso, e mais o Controle do Código-Fonte (Ctrl + Shift + G), da pra utilizar o git diretamente no vscode, fora da linha de comando)

> Git blame: extensão que mostra o último commit de cada linha e o autor que o fez



## Git commands
**git branch --set-upstream-to=origin/<branch> <branch-atual>**

> Seta uma branch para a qual sua branch atual vai ficar trackeando mudanças, como se fosse a branch do qual ela foi originada

**git commit --amend**

> Permite editar um commit já feito antes de subir para o Github

## Git tips

> Nunca altere o histórico no master, caso haja algum erro em algum dado commit, use o revert - que gera um novo commit com a reversão do commit desejado, mas não mexe no histórico

> Ou seja: git revert serve para o master e o git reset é bom para outras branches