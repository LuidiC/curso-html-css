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

- **`<margin>`**: Modifica o tamanho do espaçamento interno.
  Segue a mesma lógica no "margin", porém agora para o espaçamento interno.
  \*Observação: Poode ser usado op margin-top, margin-right e etc também para modificar especificamente apenas uma parte.
