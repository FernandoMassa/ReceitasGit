# Livro de receitas do GIT :man_cook:

## O que podemos esperar? :thinking:

​	Bom, este livro está nascendo como uma atividade prática para testar os comandos do Git e Github, mas para não ficar só fazendo coisas sem sentido, decidi criar um livro de receitas para que todos possam colaborar. Até o momento criei 3 categorias, mas nada impede que sejam criadas mais. Fiquem a vontade para fazer o que quiserem, MAS... respeitando o que os outros fizeram.

​	Se alguém estiver meio perdido, o negócio aqui é bem livre. As receitas não precisam ser de comida unicamente, claro que se não for de comida, por favor coloque na categoria correspondente e se a categoria ainda não existir, crie ela. :smile::+1: Mas não esqueça de adicionar ela no índice. 

​	Tudo bem que o esquema aqui é livre, mas vamos ter bom juízo e manter a ordem das coisas... quem sabe isto, daqui a uns anos, vira um baita livro bem bacana com um monte de receitas e dicas boas. :clown_face:

​	Para dar o pontapé inicial desta intro... seguem os comandos mais usados no git na ordem sequencial de uso. (normalmente, pelo menos pra mim. hehehe)

### Comandos Git

| Comando                                                      | Descrição                                                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| git init                                                     | Vai criar o repositório git (pasta local) dentro do local que você determinou. |
| git config --list                                            | Vai exibir toda  a configuração do seu GIT onde poderá ver se está configurado corretamente seus dados de e-mail e tudo mais. Não precisa fazer sempre. Só no caso de estar em um PC diferente do habitual ou ter perdido as configurações por algum motivo. |
| git config --global user.email "SeuEmail"                    | Assim você vai configurar seu e-mail no GIT.                 |
| git config --global user.name "SeuNome"                      | Assim você vai configurar seu nome ou apelido no GIT         |
| **Mas se eu errei na hora de fazer a configuração?**         | Daí vc faz o comendo que está logo aqui debaixo...           |
| git config --global **--unset** user.name                    | Esse comando --unset apaga o que estiver gravado no comando seguinte, por exemplo, ali é apagado o nome configurado. |
| git config --global **--unset** user.email                   | Neste é apagado o e-mail que foi configurado.                |
| git add .                                                    | Este comando adiciona todos os arquivos ao repositório       |
| git status                                                   | Vai mostrar o Status do repositório, ou seja... se tem coisa pra commitar ou não. |
| git commit -m "mensagem"                                     | Este comando é o que de fato vai jogar as informações para o repositório. Coloque uma mensagem o mais descritiva possível. |
| **E se eu quiser voltar para um commit anterior?**           | Daí terá que digitar os comandos abaixo.                     |
| git reset --hard [id commit]<br />Exemplo: <br />git reset --hard 555db00 | Então, ali no id do commit, é digitado o id que o git  mostra para cada commit. <br />Exemplo: <br />[master **555db00**] Commit 2 com ajustes nos textos.<br />Então... o codigo Alfanumérico em negrito é o id do commit. |
| git remote -v                                                | Vai listar os repositórios externos configurados.            |
| git remote add origin [URL do repositório]<br />Exemplo:<br />git remote add origin https://github.com/FernandoMassa/ReceitasGit | Vai vincular o repositório externo ao seu GIT.               |
| git checkout -b [nomebranch a ser criada]<br />Exemplo:<br />git checkout -b main | Assim você cria um branch.<br />No exemplo crio o branch MAIN, para ajustar ao novo padrão git hub onde o branch principal é o main e não o master.<br />O -b faz com que se o branch não existe, ele será criado. |
| git checkout -b [nomebranch a ser criada] [nome de onde vai copiar os arquivos]<br />Exemplo:<br />git checkout -b main master | Então, basicamente no exemplo ao lado eu estou criando o repositório main copiando o conteúdo do master. <br />Ocorre que ainda quando damos um git init, o primeiro branch que é criado, tem o nome de MASTER, assim antes de dar o commit para o Github, como lá o padrão é diferente, o melhor é já criarmos de acordo como é o padrão lá e daí puxar tudo e depois commitar. |
| Mas me deu o seguinte ERRO!!!! :cry:<br />fatal: refusing to merge unrelated histories | Não se preocupe... faça o proximo comando que vai dar certo... |
| git pull origin master **--allow-unrelated-histories**       | É bem possível que vc não precise fazer isto, mas eu tive que fazer, porque já tinha commitado pro Github meu master e daí precisei fazer um merge dele com o main. <br />Em fim, tenha certeza do que vc estiver fazendo antes de dar este comando. :smirk: |
| git merge [nome da branch que vai receber as alterações]     | Aqui vc joga pro branch as alterações que vc fez em outro branch. |
| git pull                                                     | Comando que traz as alterações que estão no github para seu repositório local. |
| git push                                                     | Comando que envia para o Github as suas alterações que **estão commitadas**. |
| git push --set-upstream origin main                          | Caso der um push e não fizer nada, provavelmente vai te dar uma sugestão tipo a daqui do lado. Copia e cola ela na linha de comando e roda. <br />Normalmente só faz isso uma vez, pode que peça novamente ao trocar de branch, pois daí o git não sabe pra que branch enviar. |
| git clone [url ....]                                         | Baixa todos os arquivos do repositório definido na url.      |



Por enquanto é isso aí, tomara que gostem, e fiquem a vontade pra complementar e adicionar novos comandos.

Fiz isto no editor Typora. Recomento muito. Ajuda pra caramba com Markdown
