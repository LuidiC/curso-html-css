Aula 02, 03 e 04

- Importante sempre manter tudo dentro do <html></html> com um TAB a mais, mantendo as boas práticas.

. <head>: Todas as configurações do HTML em si. (Ex: título do documento, linguagem, estilos de cores e etc)

. <boddy>: Os elementos em si que estão na página. (Título, imagem, botão e etc)

- F12 nos sites exibe os códigos das páginas e também é possível ver o que cada linha referencia ao passar o mouse por cima.

. <h1,h2,h3,h4,h5,h6>: Tag de título, por ordem de tamanho de acordo com os números.

\*\*\* Toda a página tem que ter única e exclusivamente um ÚNICO h1!

. <p>: Tag de parágrafo.

. <span>: Semelhante ao <p>, porém caso eu coloque um <span> do ladod de outro ele não separa em outra linha, diferente do <p>.

Usado para realçar/destacar um texto dentro de um parágrafo ou título.

Exemplo: <h4>Dicas de como usar o <spawn>H1 corretamente.</spawn></h4> (Mudaria com o CSS para amarelo o span, por exemplo)

. <b>: Deixa o texto em negrito apenas com HTML.

. <strong>: Também deixa em negrito mas o navegador entende como um trecho importante (semântica).

. <i>: Deixa em itálico.

. <em>: Deixa em itálico, porém também deixa em ênfase.

. <code>: Deixa o texto semelhante a formatação de um código.

. <blockquotes>: Formatação bem diferente, geralmente usada para demonstrar uma citação de alguém. (texto mais para o meio e um pouco diferente).

. <br>: breakline, quebra o texto para a próxima linha ou posso só utilizar outro <p>.

. <hr>: linha que vem de ponta a ponta.

. <sup>: Utilizado para demonstrar o elevando, potência.

\- Muito mais conteúdo, pesquisar no google e olhar a documentação.

Aula 05

. Para fazer uma lista, ordenada ou não, é necessário 2 estruturas <ol> (para ordenadas) ou <ul> (para desordenadas) do começo ao final da lista e para cada item é necessário colocar ele entre <li>.

. <dl>: É pouco comum, e é uma lista de descrição, depois vem o <dt>: Título e por fim o <dd>: Descrição em lista.

Aula 06

\- Link interno, aquele que você permanece dentro do domínio.

\- Link externo, aquele que te leva para fora do domínio. (Ex: do site da hashtag para o youtube)

. <a href= "link">: Para se colocar um link na palavra, item ou frase. HREF seria um atributo.

. Caso queria abrir o link do <a> em outra aba e não substituir a atual, é necessário utilizar o atributo **target="blank"**

**.** Caso queira colocar um link para percorrer a página, é necessário colocar um id no texto que você quer chegar pelo click. Em seguida coloca-se o <a href= "#nome do id">, o # é essencial!

Aula 08

. <img src="local imagem" alt="texto" />: Inserir imagens, src é o local da imagem (nome se estiver na pasta ou link na net) e alt é o texto que aparece se a imagem quebrar ou se passaro mouse em cima.

. width="" e height="": São atributos que definem a altura e largura da imagem, caso queira pode apenas definir 1 que o outro é calculado automaticamente.

. <figure>: Da um leve espaçamento na imagem e permite utilizar o figcaption (legenda na imagem)
