Para **salvarmos as alterações dos arquivos** para usar depois, usamos o comando **git stash**, esse comando reseta os estados dos arquivos para o estado original antes das mudanças.

Para vermos a **lista de stashes**, usamos o comando `git stash list`, para listar todos os stashes feitos.

Se quisermos **pegar as modificações de uma stash** usamos o comando `git stash apply STASH_NUMBER`, e para **excluir uma stash** usamos o comando `git stash drop STASH_NUMBER`, se quisermos realizar os 2 comandos de uma só vez, usamos o comando `git stash pop` tirando da stash a última alteração que foi adicionada, e a tras para o projeto.