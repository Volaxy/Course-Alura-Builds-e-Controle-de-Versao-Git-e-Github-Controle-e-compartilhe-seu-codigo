Ao juntar os trabalhos em que 2 pessoas fizeram alteração em uma mesma linha de código, o git informa que os **conflitos** precisam ser resolvidos antes de serem commitados.

Caso o **Visual Studio Code** esteja instalado e tenha sido configurado com o git, o git irá abrir o vs code no arquivo em que tiveram conflitos, e terá que ser escolhido qual das 2 alterações o git deve considerar, feito isso, será feito um **novo commit** baseado na correção dos conflitos usando `git commit`, e assim ele vai realizar o commit.

Ao tentar enviar as modificações para um repositório remoto em que **HÁ ALTERAÇÕES**, o git rejeita o **push** e avisa que o código precisa ser atualizado. Depois de inserir o comando de `git pull`, o git pedirá um **commit de merge** e assim o diretório atual será atualizado.

Antes de realizar uma alteração nova, é recomendado verificar se há alterações no repositório realizando um `git pull`.