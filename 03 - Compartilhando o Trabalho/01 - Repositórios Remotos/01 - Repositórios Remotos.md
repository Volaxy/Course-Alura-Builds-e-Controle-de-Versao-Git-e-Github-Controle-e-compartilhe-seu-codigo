Para iniciar um repositório que vai conter somente as alterações dos arquivos, sem os arquivos originais disponíveis para edição, usamos o comando `git init --bare`.

Um **repositório local** é o repositório em que alguem modifica e usa os seus arquivos, e um **repositório remoto** é onde os arquivos do projeto serão salvos para serem usados como base para os **repositórios locais**.

Para mostrar todos os **repositórios remotos** que estão vinculados com o nosso **repositório local**, usamos `git remote`.

Para adicionar um novo **repositório remoto** para vincular, usamos o comando `git remote add NOME CAMINHO`.

Para mostra o **endereço** de um **repositório remoto**, usamos o comando `git remote -v`, onde o `(fetch)` significa que ele irá buscar os dados desse caminho, e o `(push)` que ele irá enviar os dados para esse caminho.

Para clonar os arquivos de um repositório, usamos o comando `git clone CAMINHO [NOME]`.