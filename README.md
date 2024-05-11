# Prototipo_Gerador_de_Referencias_IA
Esse é o prototipo que usa o germini, para gerar referencias de artigos, materias e textos, alimentados pelo usuário, para facilitar a busca por argumentos e trechos que corroborem com sua tese.

**Lembrando:**
Essa ferramenta não substitui a leitura do Material Fonte. 
É apenas um auxiliar caso você já tenha lido varios artigos e não lembra mais em qual deles está uma fala ou argumento especifico que você encontrou, que corrabora com o seu conhecimento adiquirido.

Ele Traz consigo a formatação da referência, porém por ser um prototipo, tem poucas opções, é importante que se verifique como utilizar, para *mídia* que está sendo usada por você.

Sua primeira interação com os comandão serão para alimentar a base de dados da ferramenta, ela contem epaço para 3 documento distintos.
Você pode adicionar mais documento editando esta parte do comando:
________________________________________

Pode inserir mais adicionando o DOCUMENTO_4 
&nbsp;
  
    DOCUMENT4 = {
    "Título": input("Titulo do artigo ou prompt se for texto gerado por IA DOC 3: \n"),\n
    "Conteúdo": input("Conteudo da obra ou resposta da IA DOC 3: \n"),\n
    "Autor": input("Autor ou nome da IA generativa DOC 3: \n"),\n
    "no_publi": input("Ano de publicação da Obra ou data da versão do modelo de IA DOC 3: \n"),
    "pag": input("Numero de paginas DOC 3: \n"),
    "editora": input("Nome da editora para livros, Nome do Jornal, ou Nome da empresa criadora da IA DOC 3: \n"),
    "cidade": input("Cidade de publicação DOC 3: \n"),
    "site": input("Site ou LInk de acesso, onde está disponivel DOC 3: \n"),
    "dat_acess": input("Digite a data que acessou o documento ou texto DOC 3: \n"),
    "tipo_de_midia": input("Digite Qual a mídia do documento entre as da lista DOC 3:\n livro/site/e-book digite - 1 \n jornal digite - 2 \n IA digite - 3 \n\n")}

**PRECISA TAMBÉM ADICIONAR AQUI EM BAIXO** - DOCUMENT3, DOCUMENT4...
     
     documents = [DOCUMENT1, DOCUMENT2, DOCUMENT3, DOCUMENT4...]

_______________________________________

Ao reponder, sua segunda interação será um *input* com o seu argumento, ou pensamento

Você irá informar para o programa, o que deseja buscar dentro dos textos no bloco in[38]:


    consulta = input("Consulte um argumento: \n")


Por fim no bloco in[47], você terá acesso ao texto ou paragrafo que a IA encontrou com argumentos que se aproximam ou tem contexto com o seu

O programa, irá mostrar seu argumento, já com a **Referencia de Citação**, você pode copia-la e inserir em seu trabalho no fim de sua fala ou do paragrafo todo. 

E por fim, trará a estrutura da **Referência Bibliografica**, que você pode usar para se basear, ou copiar para seu trabalho.

Após iso, trará também a referencia usada para criar as estruturas de Referencia bibliografica.

Ex:

    Trecho do Texto Referência:
    "No entanto, a exploração espacial continua a evoluir, e quem sabe no
    futuro tecnologias e métodos inovadores permitirão que animais como
    vacas sejam enviados para outros planetas."


     Seu Argumento:
    quem sabe no futuro até as vacas possam ir ao espaço, (Germini, 1.0
    Pro 2024)


     Referencia Bibliografica:
    Google Cloud, Qual a primeira vaca a pisar na lua?.Germini Versão
    de: 1.0 Pro 2024, Inteligência Artificial, Disponivel em:
    https://gemini.google.com/app/b78ffed0e0cf7adb, Acessado em:
    11/05/2024.


    Modelos de Referências baseados em: https://usp.br/sddarquivos/arquivos/abnt6023.pdf 
    Para Mais informações acesse o link a cima. 
    Para textos em IA, ainda não há regra especifica da ABNT, 
    é importante verificar se há regras atuais para a situação.
