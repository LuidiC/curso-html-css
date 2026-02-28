# Aula 02

# Especificidade no CSS

Qual a ordem de prioridade dos seletores que herdaram as regras feitas do CSS?

No CSS, quando mais de uma regra pode ser aplicada ao mesmo elemento, o navegador decide qual usar com base na **especificidade** (prioridade do seletor).

## 🥇 Ordem de Prioridade (do menor para o maior)

1. Seletor de elemento (tag)
2. Classe (`.classe`)
3. Atributo (`[type="text"]`)
4. Pseudo-classes (`:hover`, `:focus`)
5. ID (`#id`)
6. Inline (`style=""`)
7. `!important` (força prioridade máxima)

Caso sejam utilizados 2 seletores, os "pontos" de prioridade deles se somam e a ordem será por meio disso.

# Aula 03

# Espaçamentos

- **`<margin>`**: Modifica o tamanho da margem superior e inferior e também a lateral.
  Ex: p {
  margim: 12px, 20px;
  }
  \*Observação: Caso eu coloque somente um valor, ele valerá para todos os cantos e podemos colocar até 4 valores, cada um deles correspondendo a um canto da margem.

- **`<padding>`**: Modifica o tamanho do espaçamento interno.
  Segue a mesma lógica no "margin", porém agora para o espaçamento interno.
  \*Observação: Poode ser usado op margin-top, margin-right... também para modificar especificamente apenas uma parte.

# Aula 04, 05 e 06

# Dimensões e unidades no CSS

- **`width`**: Modifica a largura (de uma div por exemplo).

- **`height`**: Modifica a altura (de uma div por exemplo).

- Medidas de _Unidades relativas_:
  _. vh:_ viewport height
  _. vw:_ viewport width
  (viewport significa a altura/largura do navegador, sempre se coloca em porcentagem de ocupação da sua tela)
  Ex: altera de acordo com o dispositivo e se está com tela cheia ou não, por exemplo.
  _. em:_ propriedade que faz com que o elemento filho herde o tamanho da regra presente no elemento pai, caso eu queria o dobro do elemento pai por exemplo é só `font-size: 2em;`
  _. rem:_ propriedade igual ao em porém sempre leva em consideração o "pai de todos", ou seja, o <html>.
  Observações:
  1. px (pixel) é uma unidade _absoluta_, ou seja, imutável.
  2. em e rem são válidos somente para elementos, não são para classes, ip e etc.

**Boa prática**: Sempre definir o html, como font-size em 62.5% e utilizar o resto do site como `rem`, isso tornará o layount responsivo pois em cada dispositivo o html pode ter um font-size padrão.

# Aula 07

# Pseudo-classes

_Pseudo-classes_ nada mais são do que uma palavra chave que irá representar o estado daquele seletore.
Ex 1: Colocamos o estado hover em um parágrafo, `p:hover {}`, isso fará com que toda vez que passarmos o mouse por cima desse determinado p o que colocamos como regra no css irá acontecer.
Ex 2: `a:link`, <a> com link, `a:visited` para <a> que já foram visitados e `a:active` para quando o usuário está clicando no link, ele muda de acordo com a regra.

\*Observação: Quando na documentação das pseudo-classes tiver o (en-US) significa que aquilo só vai funcionar quando o sistema que está sendo usado estiver em inglês dos USA.

# Aula 08

# Pseudo-elementos

_Pseudo-elementos_ são também palavras chaves que estão associadas a um seletor, mas elas representam o elemento filho daquele determinado seletor. (A primeira letra de um <p>, por exemplo)
Ex: `p::first-letter {}` modifica a primeira letra do <p>.
`p::after {}` o que entrará logo depois do parágrafo.
`p::first {}` o que entrará logo antes do parágrafo.
\*Curiosidade: Não é possível selecionar os psedo-elementos como sleecionamos textos.

# Aula 09

# Seletor Universal

O seletor universal é o `* {}`, todos os elementos ficarão as regras desse seletor. Importante falar que a ordem de prioridade dele é baixa, logo, a regra de uma tag por exemplo sobrepõe as regras desse seletor universal.
**Boa prática**: Colocar uma página sempre `* { margin:0; padding:0;}` e ajustar a posição de cada elemento manualmente.

# Aula 09

# Box Model

A propriedade border permite criar box(caixas) em diferentes estilos para os elementos da página.
Ex: div {
border: solid 3px orangered;
}

Ou você deixa sem nada e a box se adapta normalmente e deixa um pouco maior, coloca a propriedade `box-sizing: border-box;`, que você coloca exatamente o tamanho.

# Aula 11

# Sombras

Propriedade em que se coloca a shadow(sombra) e a modifica de acordo com o necessário.
Ex: /_ dentro/fora, deslocamento horizontal, deslocamento vertical, raio de desfoque, raio de propagação, cor _/
box-shadow: inset 2rem 1rem 2rem rgb(0, 0, 0, 0.2);

# Aula 12

# Novas unidades (svh, lvh, dvh)

Todas essas novas unidades vieram para solucionar um problema que acontece nas unidades de tela mobile e nas demais que variam.

_svh_ - small viewport hight
Ex: Considera a tela do usuário com a barra de pesquisa, então será depois da barra de pesquisa para baixo.

- O mais útil.
- Sempre colocar 100svh.
  _lvh_ - large viewport hight
  Ex: Considera a tela inteira, exatamente igual o vw. (Inútil)
  _dvh_ - dynamic viewport hight
  Ex: Recalcula o tempo todo a tela.
  \*Problema: Atrapalha usabilidade e diminui desempenho.
- Usado somente em casos específicos.

Temos também o svw, dvw e lvw (mesma lógica).

# Aula 13

# Elementos Arredondados

Temos a propriedade `border-radius`, que é responsável por arredondar o elemento ao qual você está aplicando a propriedade.
Ex: Caso um elemento seja um quadrado, podemos utlizar o `border-radius = 50%`, isso deixará o elemento totalmente quadrado.
