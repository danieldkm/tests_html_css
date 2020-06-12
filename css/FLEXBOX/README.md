# [Ambiente e conceitos](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Flexible_Box_Layout/Conceitos_Basicos_do_Flexbox)

Criar layout responsivos, criado e adaptado para criação de layouts

flexibilidades para adaptar a diferentes telas

# Começando com flex

Importante entender o sobre o **`flex-direction`**

row: default por padrão que mantem na mesma linha

column: mantem na vertial um abaixo do outro

row-reverse: na mesma linha porem alinha no final do container

column-reverse: na vertial porem no final do container

# Alinhamento de conteúdo

**`align-items`**: alinha verticalmente

**`justify-content`*:*** alinha horizontalmente

- ***space-between*:** adiciona espaços entre os blocos
- ***space-around*:** adiciona espaços entre os blocos e tbm no inicio e final

Para os dois:

- ***flex-start***: alinha no inicio do container
- ***flex-end*:** alinha no final
- ***center***: alinha ao centro da container

Atentar para a direção do flex, pq assim alterar o alinhamento para horizontal e vertical para cada alinhamento.

se for row então align-itens será vertical e justify será horizontal

se for column então o align-itens será horizontal e justify será vertical

# Redimensionamento

Controlar o componente para caber no espaço do container dele

- **`flex-grow` -** seta a largura dinamicamente para caber no container todo.
- **`flex-shrink`**: diz ser o nosso componente tem a capacidade de espremer dentro do container
    - 1: padrão, tenta espremer mantendo a largura que foi determinada, caso setada
    - 0: sempre irá manter a largura setada
- **`flex`**: soma do *flex-grow + flex-shrink* (ex: → flex: 1 0)

# Configurando wrap de itens

Quebra de linha no ***flexbox***

- **`flex-wrap`**: wrap
- **`align-content`:**  alinhar os elementos que tem mais de uma linha, mesma propriedade do *jusify-content*

# Ordenação

- **`order` :** cada componente quando setada a order para 0 , 1, 2.. o *css* irá ordenar dentro do container, a sequencia informada em cada flexbox

# Configurando app

resetando propriedades padrão

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```
