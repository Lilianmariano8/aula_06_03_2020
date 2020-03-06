# aula_06_03_2020
## CSS
# 1-Conceito de CSS
O Cascading Style Sheets (CSS) é uma "folha de estilo" composta por “camadas” e utilizada para definir a apresentação (aparência) em páginas da internet que adotam para o seu desenvolvimento linguagens de marcação (como XML, HTML e XHTML).
aplicaçoes 
# 2-Aplicação CSS
### Inline: aplicadas a um elemento específico num documento.
### Internal: definidas num documento específico. Permitem aplicar o estilo apenas a esse documento.
### External: definidas num ficheiro externo e associadas a vários documentos
# 3- Seletores seletores 
### Seletores com Classe
Use o atributo class em um elemento para atribuir o elemento a uma determinada classe. Muitos elementos em um documento podem pertencer a mesma classe.Em seu CSS, digite um ponto final antes do nome da classe para usar como um seletor.
Exemplo:
.um { background: moccasin; }
### Seletores com ID
♦ Casa com o elemento que tem determinado valor para o atributo id
Sintaxe: E#foo
Exemplo:
#dois { background: honeydew; }
# Seletores de Atributo
 Você pode especificar outros atributos usando colchetes. Dentro dos colchetes você insere o nome do atributo, opcionalmente seguido por um operador correspondente e um valor. Além disso, a seleção pode ser feita case-insensitive adicionando um "i" depois do valor, mas nem todos os browsers suportam esta funcionalidade ainda. Exemplos:
[disabled]
Seleciona todos os elementos com o atributo "disabled".
[type='button']
Seleciona todos os elementos do tipo "button".
[class~=key]
Seleciona elementos com a classe "key" (mas não ex: "keyed", "monkey", "buckeye"). Funcionalmente equivalente a .key.
# Seletores de pseudo-classes
É uma palavra-chave adicionada aos seletores que especifica um estado especial do elemento a ser selecionado. Por exemplo  :hover, aplicará um estilo quando o usuário passar o mouse sobre o elemento especificado pelo seletor.
Syntax
selector:pseudo-class {
  property: value;
} 
Lista de pseudo-classes
:link
:visited
:active
:hover
:focus
:first-child
:last-child
:nth-child
:nth-last-child
:nth-of-type
:first-of-type
:last-of-type
:empty
:target
:checked
:enabled
:disabled
### Seletor universal
aplica estilos a elementos de qualquer tipo. A partir do CSS3, o asterisco pode ser combinado com namespaces : ... |* - aplica a todos os elementos que não tem namespaces declarados.
Não existe uma padronização para essa folha de estilos e cada navegador implementa sua própria folha de estilos nativa. Como consequência ocorrem inconsistências de renderização, em relação a estilização básica, entre navegadores.

Destas inconsistências a que produz maiores transtornos é a não padronização dos valores para as propriedades margin e padding.

A principal utilização do seletor universal é "zerar" essas propriedades para todos os elementos da marcação. Como consequência o autor terá que definir explicitamente para cada elemento, na sua folha de estilos, aqueles valores.

CSS
* {
  margin: 0;
  padding: 0;
  }
  ### Seletor tipo
Sintaxe: E
Usado para estilizar os elementos da marcação que são de um mesmo tipo; por exemplo: elemento do tipo p (parágrafo), do tipo div, do tipo ol, do tipo strong, e assim por diante.Exemplo:

  ## Seletores de atributo
  ### Presença de um atributo
♦ Casa com elementos que contenham um determinado atributo
Sintaxe: E["foo"]

### valor de um atributo
♦ Casa com elementos com determinado valor de atributo
Sintaxe: E[foo="bar"]
## valor de um atributo pertence a uma lista de valores separados por espaço
♦ Casa com elementos cujo valor de atributo pertença a uma lista de valores separados por espaço
Sintaxe: E[foo~="bar"]
Exemplo:
*[class~="b"] { color: orange; }

### valor de um atributo começa com string
♦ Casa com elementos cujo valor de atributo começa com uma determinada string
Sintaxe: E[foo^="bar"]
Exemplo:
p[class^="a-"] { color: blue; }



### valor de um atributo termina com string
♦ Casa com elementos cujo valor de atributo termina com uma determinada string
Sintaxe: E[foo$="bar"]
Exemplo:
*[class$="-r"] { color: red; }
## Seletores do tipo pseudo-classe
### elemento raiz
♦ Casa com o elemento raiz do documento
Sintaxe: :root
Exemplo:
:root { color: blue; }
### enésimo filho
♦ Casa com o elemento que é o enésimo filho do seu elemento pai
Sintaxe: E:nth-child(n)
Exemplo:
li:nth-child(4) { color: red; }
li:nth-child(2n+1) { color: blue; }
li:nth-child(5n) { color: green; }
## enésimo filho de trás para frente
♦ Casa com o elemento que é o enésimo filho do seu elemento pai, contado de trás para frente na marcação
Sintaxe: E:nth-last-child(n)
Exemplo:
li:nth-last-child(3n) { color: salmon; }
### enésimo irmão do seu tipo
♦ Casa com o elemento que é o enésimo irmão (filhos do mesmo elemento pai) do seu tipo
Sintaxe: E:nth-of-type(n)
Exemplo:
p:nth-of-type(2n+1) { color: red; }
### enésimo irmão do seu tipo de trás para frente
♦ Casa com o elemento que é o enésimo irmão (filhos do mesmo elemento pai) do seu tipo, contado de trás para frente na marcação
Sintaxe: E:nth-last-of-type(n)
Exemplo:
p:nth-last-of-type(2n+1) { color: red; }
### primeiro filho
♦ Casa com o elemento que é o primeiro filho do seu elemento pai
Sintaxe: E:first-child
Exemplo:
div :first-child {
    color: red;
}
## último filho
♦ Casa com o elemento que é o último filho do seu elemento pai
Sintaxe: E:last-child
Exemplo:
div p:last-child { color: blue; }
## primeiro do mesmo tipo
♦ Casa com o elemento que é o primeiro irmão (filhos do mesmo elemento pai) do mesmo tipo
Sintaxe: E:first-of-type
Exemplo:
div p:first-of-type { color: red; }
### último do mesmo tipo
♦ Casa com o elemento que é o último irmão (filhos do mesmo elemento pai) do mesmo tipo
Sintaxe: E:last-of-type
Exemplo:
div p:last-of-type { color: blue; }
### único filho
♦ Casa com o elemento que é o único filho do seu elemento pai
Sintaxe: E:only-child
Exemplo:
p:only-child { color: orange; }























   

  
  
  
  
  
  








