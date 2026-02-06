# Aula 01

## CSS

- _Cascading Style Sheets_
- _Cascading_ pois vários arquivos de estilização podem estar ativos no mesmo documento ao mesmo tempo.
- _Style Sheet_: é o nome dado ao arquivo de estilização que contém os _seletores_(formas de identificar um elemento em uma página, em quem irei realizar a formatação) e as _regras de estilização_(aquilo que irei fazer exatamente na formatação).

## Informações do CSS

- Nome do arquivo padrão é "style.css"
- No CSS é possível formatar os seletores, sendo eles as Tags, os IDs e as Classes (sendo os últimos 2 os mais importantes).
- _ID_: atributo único, só pode ser usado em um elemento dentro de uma página.
- _p.classe_: exemplo de seletor que só será alterado na página se for um <p> que esteja na class="classe".
- _p .classe_: exemplo de seletor que só será mudado se dentro do <p> tiver algum elemento com a class="classe", mas que não seja o <p> em si.

## Tipos de formatação no CSS

**1. Inline**

- CSS aplicado diretamente na tag HTML.
- Ex: <p style="color:red;">Texto</p>
  ➡️ Rápido, mas ruim de manter.

**Internal (Interno)**

- CSS dentro da própria página, na tag <style>.
- Ex: dentro do <head>.
  ➡️ Organiza melhor, mas só vale pra aquela página.

**External (Externo)**

- CSS em arquivo .css separado, ligado com <link>.
  ➡️ Melhor prática: reutilizável e fácil de manter.

  ## Comandos e atalhos

  **<link rel="stylesheet" href="nome_do_arquivo.css" />**: forma de linkar o arquivo externo CSS ao arquivo HTML. (Colocar no head, Depois do title)
  style="color: " -> Escolhe a cor
  style="font-size " -> Escolhe o tamanho da fonte, podendo colocar em px por exemplo. (ex:style="font-size: 25px")

  **#ID**: Caso eu queira alterar o CSS apenas de um item, basta eu colocar a "#nomeID" e depois a regra de utilização no arquivo CSS que o elemento será formatado.

  **p span{}**: É possível juntar 2 seletores de tag e somente aquele que obedecer todas as regras presentes terá alguma mudança. (Podemos juntar Tags + classes, IDs + classes e etc...)

  **font-family: "Roboto", sans-serif;**: Mudar a fonte para a que deseja (nome em '') e o "sans-serif" seria o sem aqueles tracinhos para fora da palavra.

  **font-style: italic;**: Deixa em itálico.
  **font-weight: bold;**: Deixa cada vez mais pesado, ou seja, em netrito.

  **line-height**: Altera a altura da linha do texto.
  - Caso eu coloque uma tag span e depois dela coloque um ".", já puxará automaticamente a estrutura da class="" e o nome das classes presentes também.

  **text-transform: uppercase/lower...;**:Altera se está em maiúsculo, minúsculo, somente a primeira maiúsculo e etc.

  **text-decoration: none;**: Tira o sublinhado de links por exemplo.

  **text-decoration-color:...;**: Escolhe a cor da linha, caso não coloque a cor o texto usará a cor padrão do texto atual.
