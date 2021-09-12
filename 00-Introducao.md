# Livro de receitas do GIT :man_cook:

## O que podemos esperar? :thinking:

​	Bom, este livro está nascendo como uma atividade prática para testar os comandos do Git e Github, mas para não ficar só fazendo coisas sem sentido, decidi criar um livro de receitas para que todos possam colaborar. Até o momento criei 3 categorias, mas nada impede que sejam criadas mais. Fiquem a vontade para fazer o que quiserem, MAS... respeitando o que os outros fizeram.

​	Se alguém estiver meio perdido, o negócio aqui é bem livre. As receitas não precisam ser de comida unicamente, claro que se não for de comida, por favor coloque na categoria correspondente e se a categoria ainda não existir, crie ela. :smile::+1: Mas não esqueça de adicionar ela no índice. 

​	Tudo bem que o esquema aqui é livre, mas vamos ter bom juízo e manter a ordem das coisas... quem sabe isto, daqui a uns anos, vira um baita livro bem bacana com um monte de receitas e dicas boas. :clown_face:

​	Para dar o pontapé inicial desta intro... seguem os comandos mais usados no git na ordem sequencial de uso. (normalmente, pelo menos pra mim. hehehe)

### Comandos Git

| Comando                                              | Descrição                                                    |
| ---------------------------------------------------- | ------------------------------------------------------------ |
| git init                                             | Vai criar o repositório git (pasta local) dentro do local que <br />você determinou. |
| git config --list                                    | Vai exibir toda  a configuração do seu GIT onde poderá ver <br />se está configurado corretamente seus dados de e-mail e <br />tudo mais. Não precisa fazer sempre. Só no caso de estar<br />em um PC diferente do habitual ou ter perdido as configurações<br />por algum motivo. |
| git config --global user.email "SeuEmail"            | Assim você vai configurar seu e-mail no GIT.                 |
| git config --global user.name "SeuNome"              | Assim você vai configurar seu nome ou apelido no GIT         |
| **Mas se eu errei na hora de fazer a configuração?** | Daí vc faz o comendo que está logo aqui debaixo...           |
| git config --global **--unset** user.name            | Esse comando --unset apaga o que estiver gravado no <br />comando seguinte, por exemplo, ali é apagado o nome configurado. |
| git config --global **--unset** user.email           | Neste é apagado o email que foi configurado.                 |
| git add .                                            | Este comando adiciona todos os arquivos ao repositório       |
| git status                                           | Vai mostrar o Status do repositório, ou seja... se tem <br />coisa pra commitar ou não. |
| git commit -m "mensagem"                             | Este comando é o que de fato vai jogar as informações <br />para o repositório. Coloque uma mensagem o mais<br />descritiva possível. |
| **E se eu quiser voltar para um commit anterior?**   | Daí terá que digitar os comandos abaixo.                     |
| git reset --hard [id commit]                         | Então, ali no id do commit, é digitado o id que o git <br />mostra para cada commit. <br />Exemplo: <br /> |





