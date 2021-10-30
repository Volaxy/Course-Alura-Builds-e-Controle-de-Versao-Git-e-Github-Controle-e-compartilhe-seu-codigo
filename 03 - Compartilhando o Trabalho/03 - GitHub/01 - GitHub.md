No **GitHub**, poderemos criar uma conta, e a partir daí passar a criar repositórios Git de forma muito simples. Feito o login, independentemente do quão familiar você esteja com o site, é possível clicar no símbolo de **`+`** localizado no canto superior direito para criar um novo repositório, por meio da opção "New repository".

Na nova página, poderemos definir o criador do repositório (*Owner*) e o seu nome (*Repository name*), que pode ser qualquer um. Daremos uma descrição (*Description*). O repositório pode ser configurado como público ou privado, dependendo da conta que tivermos. Normalmente, os repositórios privados só ficam disponíveis para usuários pagantes. Caso você seja usuário de plano grátis, será possível apenas criar repositórios públicos.

Após clicarmos no botão "Create repository" no fim da página, seremos redirecionados a outra, com dicas sobre como poderemos criar um novo repositório por linhas de comando, entre outras. No nosso caso, já temos um repositório local, arquivos commitados, e tudo o mais, então optaremos pelo envio deste repositório, com **`git remote add origin git@github.com:CViniviusSDias/alura-git.git`**, uma sintaxe talvez não muito familiar, para o qual precisaríamos definir chave de acesso, algo mais seguro, porém complicado.

Na parte superior desta página, onde se lê "Quick setup — if you've done this kind of thing before", selecionaremos "HTTPS" em vez de "SSH", de forma que, toda vez que precisarmos enviar os dados ou adicionar um repositório durante envio ou quando formos trazê-lo de volta, precisaremos digitar uma senha.

No Git Bash, colaremos o comando, feito isso, no site do GitHub é indicado que devemos enviar os dados do repositório com **`git push -u origin master`**, cujo **`-u`** define que, sempre que usarmos **`git push`** e estivermos na **master**, o envio seja feito para **origin**. Ou seja, a partir de então poderemos executar simplesmente **`git push`**.

É aconselhavel não seguir esta abordagem, e sempre digitar qual o repositório e qual branch você quer enviar, para manter um controle maior do nosso lado. Sendo assim executo git push origin master.

O GitHub é uma plataforma muito poderosa, e faz muito mais do que simplesmente disponibilizar repositórios remotos: conseguimos configurar colaboradores no projeto, para que outros usuários de GitHub possam fazer commits diretamente, entre outras vantagens.

Com o GitHub, podemos ter repositórios remotos públicos e privados gratuitos para armazenar e compartilhar o código dos nossos projetos.

O GitHub fornece muitas outras funcionalidades bem legais.