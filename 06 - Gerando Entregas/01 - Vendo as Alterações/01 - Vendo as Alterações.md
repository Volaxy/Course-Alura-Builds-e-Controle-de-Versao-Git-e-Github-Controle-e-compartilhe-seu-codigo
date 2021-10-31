No momento de finalizarmos, queremos verificar o que houve em cada commit, para garantir que nenhum bug foi adicionado no projeto, e entender o que de fato cada commit gerou no código. Como conferiremos as diferenças entre commits?

Existe um comando do Git, bem interessante e poderoso, que é o **`git diff`**, capaz de exibir estas diferenças. Ao tentarmos executá-lo, porém, nada é exibido.

Isso porque por enquanto não há nada alterado no nosso código, que não tenha sido salvo. Então, para entendermos as diferenças entre dois commits, precisaremos informar quais são, no caso, **ea539b3** até (**..**) **6ca12ac**. Por meio deste comando, visualizamos todas as alterações feitas, marcadas em cores diferentes.

Além disso, caso estejamos modificando algo, como acresentando um novo curso na listagem, no código, e queiramos verificar o que foi alterado, poderemos simplesmente usar o **`git diff`**, que nos mostra o que foi alterado e que ainda não foi adicionado para commit. Mas a partir do momento em que adicionamos o arquivo, este comando não nos mostra mais o que existe de diferente.