# Desafio-1-Escola-DNC
Primeiro desafio da escola DNC (HTML,CSS e JS)

Primeiramente criei um arquivo Index.html com html5 para facilitar o desenvolvimento da pagina.

Após isso comecei a configurar o head linkando um arquivo .css para estilizar a pagina.

logo abaixo, no head, linkei algumas fontes a serem ultilizadas no projeto através do google fonts. o proprio google fonts já fornece o codigo pronto para ser inserido no HTML.

Ainda no head, inseri o titulo da minha pagina.

partindo para o body, comecei com a primeira div para o menu superior da pagina (usando o id "menu superior" para posteriormente edita-lo no .CSS)

ps: eu organizo todo o projeto usando comentarios através da tag <!--""-->. desta forma, o desenvolvimento fica muito mais organizado.

ja no css, coloquei a margem em zero e estabeleci a fonte como "inter" usando o "*" para que essas configurações fossem aplicadas a todo o projeto.

Usei a cor de fonte e backgroud color igual ao modelo do Figma. ajustei todo o padding e tamanho das fontes do h1 e p (ambos com suas respectivas ids no HTML); também ajustei a margem inferior do h1 para conferir o espaçamento adequado entre o p1 .

partindo para a segunda parte da pagina, o menu informacional, criei uma primeira div (menu-informacional) para editar o brackgroud e toda a parte de padding e margem e uma segunda div ("info" criada dentro da div "menu-informacional") para editar a parte dos textos.

De acordo com o modelo no Figma, os titulos deveriam ser divididos e 2 partes cada um, uma vez que parte do texto usava um tamanho de fonte e um fonte-weight diferente além de existir uma quebra de texto.

para isso, divid o h1 e duas partes usando a tag <span> e dando quebra de texto com a tag <br>. atribui classes (sim, classes, afinal o menu informacional possuia 3 titulos e usando as classes eu poderia atribuir uma mesma alteração a todos os elemntos desejados) diferentes para o h1 e span para que eu pudesse editalos de maneira individual. (você pode observar com  mais clareza esse procedimento entre as linhas 18 e 28 do index.html).

alinhei os elemntos atraves do display: grid e grid-auto-flow: column; deixando os elemntos alinhados em colunas, seguindo o modelo do Figma.

Na div da parte central do site (linha 33),  também organizei os elementos em colunas atraves do grid no CSS. também dei um margin-bottom de 100px.

novamente o h1 teve que ser dividido em duas parte através da tag <span>, <br> e também com ids diferentes para que cada parte fosse editada separadamente.

Essa parte continha uma imagem. Criei um arquivo .svg com a imagem do Figma e inseri a mesma no HTML com a tag <img>. ajustei a width e height no CSS(id="imagem-central").

Partindo então para a parte do formulário (primeiramente criei uma div para essa etapa id="formularios"), usei a tag <form> com o método post (method = "post"), para que as informções do formulário fossem postadas nas planilhasa do Google Sheets através do sheet monkey (action="link do sheet monkey"). 

Como de costume, estilizei toda essa parte no CSS, deixando o "text align" em "center" para que os inputs ficassem centralizados. Também configurei toda a parte de padding e coloração

Na parte de input (não foi necessário criar uma id especifica aqui), foram abertas 3: uma para email, outra para nome, e outra pra registar hora e data da coleta dos dados. esta ultima fica oculta ao front-end atraves do comando type="hidden". Praticamente toda essa parte de form é diponibilizada pronta pelo Sheet monkey. É importante também adicionar um placeholder. Essa informação será exibida dentro do campo para que o usuário digite a informação (ex: "digite seu email", "digite seu nome").

o botão (button) é do tipo submit (type="submit"), que ao ser clicado irá enviar as informações para as planilhas. entre a abertura e o fechamento da tag <button>, deve ser digitado o texto que o botão irá exibir (no caso "Fale Conosco")

no css, ajustei as dimensões do botão, a fonte e as cores de acordo com o modelo do figma. removi as bordas (border= 0px;) usei o comando "border-radiu= 5px" para deixar as pontas do botão arredondadas. o cursor foi mudado para o estilo "pointer" 

Já o button-hover serve para adicionar uma animação ao botão assim que o cursor do mouse for colocado em cima dele. o comando "transform:translateY(-7px) ;" fará o botão se mover 7 pixels acima; o "box-shadow: 0px 15px 20px #1a2225;" é referente ao tamanho e a cor da sombra que a animação fará. E por ultimo o "transition-duration: 0.5s;" é o tempo em que a animação durará.

fim ;) 