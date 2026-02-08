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

- **`<var>`**: Tag usada para mostrar algo como uma variável.

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

# Aula 05

# Formulário

Todos os elementos de um formulário precisam estar dentro da tag `<form action="">` (action: para onde as infromações irão parar, URL por exemplo). Existem diversas maneiras de personalização quando estamos falando de formulário, por isso é sempre importante checar a documentação e utilizar aqui que for melhor.

- **`<input>`**: Utilizado para o usuário escrever, inputar algo, existem vários tipos de input, importante olhar na documentação. (não precisa estar dentro da tag `<input>` para funcionar)
  Ex: <input id="nome" name="nome" type="text" />
  O formulário salavrá a informação como nome.
  Obs: De acordo com o "name" que escolhemos para o nosso input, ele puxa infomações de outros formulários que já preenchemos naquele navegador com inputs que possuiam o mesmo "name". (sempre coloque em inglês)
  Ex 2: <input id="nome" name="nome" type="text" placeholder="Seu nome"/>  
  "placeholder": escrita que aparece no input antes do usuário digitar algo.
  - **`<pattern>`**: é um atributo que só pode ser utilizado dentro de um input, utilizado para fazer validações no input de acordo com a regra daquele determinado campo.

- **`<label>`**: Tag utilizada como uma legenda ou rótulo para um elemento de formulário, como um <input> ou <textarea>. Ela serve para identificar visualmente o que o usuário deve inserir em cada campo.
  Acessibilidade: Permite que leitores de tela identifiquem corretamente qual texto descreve qual campo de entrada para usuários com deficiência visual.

- **`<button>`**: Tag que cria um botão, possui 3 types:
  . type="button": Ele não faz nada sozinho — só executa algo se você mandar, normalmente com JavaScript.

. type="submit": É o tipo padrão do <button> quando ele está dentro de um <form>.
Quer enviar os dados do formulário.
Quer disparar a ação definida no action do <form>.

. type="reset": Ele limpa todos os campos do formulário, voltando para os valores iniciais.
