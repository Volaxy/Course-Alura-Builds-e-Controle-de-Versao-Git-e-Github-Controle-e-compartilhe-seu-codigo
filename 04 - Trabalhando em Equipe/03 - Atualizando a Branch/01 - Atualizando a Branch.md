Anteriormente, vimos como unir o trabalho de duas branches desenvolvidas separadamente. No entanto, não queremos gerar um commit a mais, de merge, dependendo da estratégia utilizada para gerar os commits, isto pode acabar atrapalhando ou "poluindo" o log. Assim, o que queremos é atualizar a branch **master** com os commits da branch **titulo**, de modo a termos cada commit específico na linha de desenvolvimento **master**.

Na ferramenta Visualizing Git, faremos um **`git checkout -b titulo`** para gerarmos dois commits (**`git commit`** duas vezes). Na branch **master**, corrigimos um bug, portanto geraremos outro commit. E então, da branch **titulo**, queremos trazer os demais commits para antes de **master** atualizando as duas branches.

Para isto, estando na **master**, queremos basear esta branch em **titulo**, assim, executaremos **`git rebase titulo`**, e o Git pegará os commits na branch **titulo**, atualizando **master**, que possui todos os commits contidos em **titulo**, além do commit que havia nela mesma. Deste modo, geramos uma única linha, sem confusões.

No Git Bash, executaremos **`git log`** novamente, e teremos a informação de commit de merge; de que forma conseguiremos visualizar isso de forma mais interessante? Se digitarmos **`git log --graph`**, serão exibidas linhas específicas representando o desenvolvimento, uma boa alternativa ao Visualizing Git.

Vamos fazer uma alteração na branch **titulo**, com **`git checkout titulo`**, e no VS Code alteraremos a primeira letra de "Cursos" para que fique em maiúscula. Adicionaremos o arquivo e o commitaremos, e depois iremos à branch **master** para trazermos os commits de **titulo** para ela, por meio de **`git rebase titulo`**.

O **`rebase`** atualiza a branch, mantendo o trabalho dela como sendo o último, para que não se gere confusão. Com isso, temos as correções realizadas tanto no título quanto no master.