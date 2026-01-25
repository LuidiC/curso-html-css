# Aula 01

## 🌐 Tipos de Páginas

- **Página Dinâmica**: Igual para todos os usuários.
- **Página Estática**: Muda de usuário para usuário, personalizada para cada um.
  - **Exemplos**: YouTube, Instagram, Facebook.

## 💻 Desenvolvimento Front-end

- **HTML**: Esqueleto do site
  - Títulos, parágrafos, imagens, vídeos, etc.

- **CSS**: Estilização do site
  - Cores, tamanhos, espaçamentos, sombras, etc.

- **JavaScript**: Interatividade do site
  - Mostrar/ocultar informações
  - Carrosséis
  - Contadores em sites

> 📊 **Curiosidade**: Cerca de **98,3%** das páginas na internet utilizam JavaScript.

---

# Aula 03

## 📚 Boas Práticas de Estudo

- Utilizar bastante fóruns, especialmente o **Stack Overflow**.
- Pesquisar conteúdos no Google **em inglês** para melhores resultados.
- Consultar documentações oficiais.
  - Exemplo: documentação de CSS no **MDN Web Docs**.

## 🖱️ Conceitos Importantes

- **Hover**: Ação de passar o mouse sobre um elemento.
  - Exemplo: exibir uma borda ao passar o mouse usando CSS.

---

# Aula 02, 03 e 04

## 🧱 Estrutura Básica do HTML

- É importante manter **todo o conteúdo dentro da tag `<html></html>`**, usando **indentação (TAB)** correta para seguir boas práticas.

- **`<head>`**: Contém as configurações do documento HTML.
  - Ex: título da página, linguagem, estilos, metadados etc.

- **`<body>`**: Contém os elementos visíveis da página.
  - Ex: títulos, imagens, botões, textos etc.

- Pressionar **F12** em um site abre o **DevTools**, permitindo:
  - Visualizar o código da página
  - Ver a que elemento cada linha se refere ao passar o mouse

## 🏷️ Principais Tags de Texto

- **`<h1>` até `<h6>`**: Tags de título (ordem decrescente de tamanho).

> ⚠️ **Regra importante**: Toda página deve ter **um único `<h1>`**.

- **`<p>`**: Parágrafo.

- **`<span>`**: Semelhante ao `<p>`, porém **não quebra linha**.
  - Usado para destacar partes de um texto.

**Exemplo:**

```html
<h4>Dicas de como usar o <span>H1</span> corretamente.</h4>
```

_(O `<span>` pode ser estilizado com CSS, por exemplo, mudando a cor para amarelo.)_

- **`<b>`**: Texto em negrito (apenas visual).
- **`<strong>`**: Texto em negrito com **importância semântica**.
- **`<i>`**: Texto em itálico.
- **`<em>`**: Texto em itálico com **ênfase semântica**.
- **`<code>`**: Texto com aparência de código.
- **`<blockquote>`**: Usada para citações (formatação diferenciada).
- **`<br>`**: Quebra de linha.
- **`<hr>`**: Linha horizontal de ponta a ponta.
- **`<sup>`**: Texto sobrescrito (potência, exponencial).

> 📌 Há muito mais conteúdo — pesquisar no Google e consultar a documentação oficial.

---

# Aula 05

## 📋 Listas em HTML

- Para criar listas é necessário usar:
  - **`<ol>`** → Lista ordenada
  - **`<ul>`** → Lista não ordenada

- Cada item da lista deve estar dentro de **`<li>`**.

### 📘 Lista de Descrição

- **`<dl>`**: Lista de descrição (menos comum)
- **`<dt>`**: Título/termo
- **`<dd>`**: Descrição do termo

---

# Aula 06

## 🔗 Links

- **Link interno**: Permanece dentro do mesmo domínio.

- **Link externo**: Leva para outro site.
  - Ex: do site da Hashtag para o YouTube.

- **`<a href="link">`**: Cria um link.
  - `href` é um **atributo**.

- Para abrir o link em outra aba:

```html
<a href="link" target="_blank">Texto</a>
```

- Para criar um link que navega dentro da própria página:
  1. Definir um `id` no elemento de destino
  2. Usar `#id` no `href`

```html
<a href="#secao">Ir para seção</a>
```

> ⚠️ O `#` é essencial.

---

# Aula 08

## 🖼️ Imagens

- **`<img src="" alt="" />`**: Inserção de imagens
  - `src`: caminho da imagem (local ou URL)
  - `alt`: texto alternativo (acessibilidade e erro de carregamento)

- **`width`** e **`height`**:
  - Definem largura e altura
  - Se apenas um for definido, o outro é calculado automaticamente

- **`<figure>`**:
  - Cria um leve espaçamento
  - Permite usar **`<figcaption>`** para legenda da imagem
