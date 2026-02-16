# Aula 01

# Aprofundamento do HTML

- _Componentes_: Formulários, Tabelas, iFrames, Paginação e Carrosel.

# Aula 02

# Tags diferenciadas

- **`<blockquote>`**: Usada para citações EM PARÁGRAFOS, podendo ter também a versão `<blockquote cite="link">`, demonstarnado dentro do cite o link de onde pegou a citação, porém isso não aparece para ninguém na página em si.

- **`<q>`**: Coloca citação no MEIO DE UMA FRASE, com "Fulano disse isso". (cite pode ser usado também)

- **`<cite>`**: Coloca no meio dessa tag quem é a pessoa que citou aquilo.

- **`<abbr>`**: Usado para mostrar ao usuário quando passa por cima da palavra abreviada, qual o significado total dela. Ex: HTML (Hyper Text Markup Language)

- **`<address>`**: Tag usada para demonstrar informações de contato. (celular, endereço, e-mail e etc)

- **`<pre>`**: Tag usada para o HTML ler exatamente os espaços colocados no código.
  Ex: <pre><code> function() {
  console.log("Olá, mundo!")
  } </code></pre>
  Cascading Style Sheets
- **`<kbd>`**: Tag para retratar teclas do teclado.
  Ex: <kbd>CTRL + K</kbd>
  - **`<time datetime="">`**: Tag para especificar ao navegador que é uma data.
    Ex: <time datetime="26-02-05">Dia 5 de Fevereiro de 2026</time>

# Aula 04

# Estrutura do HTML

Determinadas estruturas que vimos até agora não deveriam ficar simplesmte jogadas no código, mas sim organizadas em certas estruturas.

Como exemplo temos:

- **`<header>`**: Utilizado para representar todo o cabeçalho. (Usado apenas 1 vez por página)

- **`<footer>`**: Utilizado para representar a navegação principal da página. (Usado apenas 1 vez por página)

- **`<main>`**: Representa o conteúdo principal do site, o conteúdo inteiro em si. (onde todas as outras seções tirando `header`, `nav` e `footer` estão)

- **`<article>`**: Utilizado para representar um artigo.

- **`<aside>`**: Utilizado para representar algo que não necessariamente está relacionado ao conteúdo principal do site.

- **`<section>`**: Utilizado no main quando não consegue se enquadrar no `<aside>` ou `<article>` porém ainda sim você quer dividir em uma seção.

- **`<div>`**: Tag utilizada para separar alguns elementos da página em blocos, porém sem uma semântica ou algo específico. (possível usar uma `<div>` dentro da outra). Quando coloco 2 <divs> seguidas uma da outra os elemetos de cada uma ficarão agrudos abaixo da outra.

- **`<footer>`**: Utilizado para representar o rodapé.

# Aula 05 e 06

# Formulário

Todos os elementos de um formulário precisam estar dentro da tag `<form action="">` (action: para onde as infromações irão parar, URL por exemplo). Existem diversas maneiras de personalização quando estamos falando de formulário, por isso é sempre importante checar a documentação e utilizar aqui que for melhor.

- **`<input>`**: Utilizado para o usuário escrever, inputar algo, existem vários tipos de input, importante olhar na documentação. (não precisa estar dentro da tag `<input>` para funcionar)
  Ex: <input id="nome" name="nome" type="text" />
  O formulário salavrá a informação como nome.
  Obs: De acordo com o "name" que escolhemos para o nosso input, ele puxa infomações de outros formulários que já preenchemos naquele navegador com inputs que possuiam o mesmo "name". (sempre coloque em inglês)
  Ex 2: <input id="nome" name="nome" type="text" placeholder="Seu nome"/>  
  "placeholder": escrita que aparece no input antes do usuário digitar algo.
  - **`pattern`**: É um atributo que só pode ser utilizado dentro de um input, utilizado para fazer validações no input de acordo com a regra daquele determinado campo. (Dica: Olhar no regex101.com)
  - **`required`**: Atributo que faz com que seja necessário algo no input para ser enviado.
  - **`title`**: Atributo que será responsável por mostrar o que está escrito na caixa de erro ao enviar um input errado.

- **`<label>`**: Tag utilizada como uma legenda ou rótulo para um elemento de formulário, como um <input> ou <textarea>. Ela serve para identificar visualmente o que o usuário deve inserir em cada campo.
  Acessibilidade: Permite que leitores de tela identifiquem corretamente qual texto descreve qual campo de entrada para usuários com deficiência visual.

- **`<button>`**: Tag que cria um botão, possui 3 types:
  . type="button": Ele não faz nada sozinho — só executa algo se você mandar, normalmente com JavaScript.

. type="submit": É o tipo padrão do <button> quando ele está dentro de um <form>.
Quer enviar os dados do formulário.
Quer disparar a ação definida no action do <form>.

. type="reset": Ele limpa todos os campos do formulário, voltando para os valores iniciais.

# Aula 07 e 08

# Tabela

- **`<table>`**: Cria uma tabela ao inserir seus elementos.
- **`<caption>`**: Cria legenda da tabela, não é obrigatório.

- **`<tr><td></td></td>`**: Colocar cabeçalho na tabela. (head)

- **`<tr><td></td></td>`**: Colocar algum elemento na tabela. (body)
  Exs: <tr>
  <td>Informação 1</td>
  </tr>
  <tr>
  <td>Informação 2</td> 
  -Duas linhas diferentes

  <tr>
  <td>Informação 1</td>
  <td>Informação 2</td>
  </tr> 
  -Mesa linha, porém 2 colunas diferentes.
  - **`<colgroup></colgroup>`**: Deixa em negrito todos os <th>, permite uma personalização específica de cada coluna com o **`<col>`**. (cada <col> se refere a uma coluna)
  <col span="número_colnas" class="" ou style=regra...>: Para quantas colunas específicas eu quero que aquela determinada regra se replique.

  # Aula 09

  # iFrames

  Embedar: Quando pegamos algo feito em outra página e trazemos para a nossa página, geralmente feito por meio do iFrame.

- **`<iframe src="" frameborder="0"></iframe>`**: Tag que cria um novo navegador dentro da sua própria página, um novo contexto de navegação dentro da página. Improta outra página para a sua.
  Utilidades: Posso pegar um vídeo do YouTube e colocar dentro da minha página, o Google Maps e etc.

# Aula 10

# Dialog

É a forma mais fácil de se fazer pop-ups nas páginas web.
Obs: Quase sempre será necessário o JavaScript para utiizar essa tag.

# Aula 11

# Selectedcontent

Até o momento do curso era limitado, portanto, exige muitas coisas para funcionar.
Ex: Estrutura básica junto com algumas coisas no css para funcionar:

<select id="plan">
<button><selectedcontent></selectedcontent></button>

                <option value="pro" selected>
                  <span class="row"
                    ><span class="badge b2">P</span><strong>Pro</strong
                    ><span>• Projetos sérios</span></span
                  >
                </option>

                <option value="enterprise">
                  <span class="row"
                    ><span class="badge b4">E</span><strong>Enterprise</strong
                    ><span>• Escala máxima</span></span
                  >
                </option>
                </select>
