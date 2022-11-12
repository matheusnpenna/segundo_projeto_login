# Orientações e notas sobre a correção:

<br />

## A partir dos próximos, subir os arquivos do gulp e do node: 
## gulpfile.js e o package.json

<br>

## Criei uma pasta chamada correção e coloquei a minha implementação do projeto
## O senhor pode ver como eu faria essa página e as práticas que utilizei
## Estará comentado o por que utilizei cada estratégia logo acima do trecho de código

<br>

# Notas sobre seu projeto:

<br>

## Gostei muito!!! Parabéns tio!

<br>

## Pontos positivos:
- A responsividade do projeto funciona bem;
- Conseguiu realocar os elementos sem precisar duplicar código, utilizando somente CSS
- Usou muitos recursos do CSS e entendeu bem como usar flex-box
- Se preocupou com micro-interações implementando o hover no login
- Importou a fonte diretamente no CSS
- Soube mudar o esitlo do placeholder dos inputs utilizando css
- Foi inteligente utilizar um font-size: 2vw no h1, mas gostei muito da lógica e é uma técnica recomendada na documentação do W3Schools. O problema é que quase sempre vai ficar muito pequeno no mobile, eu prefiro utilizar px e setar como eu quero que fique no mobile por uma media query



## Pontos negativos:
- No responsivo a tela ficou apertadinha por conta do display flex
  - Explicação:
    - Quando utilizamos flexbox e centralizamos no meio, caso os elementos não tenham width e height absolutos no css, o flexbox vai empurrar tudo para que o conteúdo obedeça o alinhamento utilizado. Assim, como os inputs tem width relativo (width: 100%), a largura dele é 100% do que o elemento logo acima disponibilizar, logo, a largura dele vira a largura em que o flexbox deixa ele ter na tela;
    - Como na classe main-login foi aplicado no mobile com um flex-direction: column e utilizado align-items: center. No mobile tudo é empurrado para o meio reduzindo de tamanho dos inputs que tem width: 100%;
    - Para corrigir isso, coloque width absoluto invés de relativo ou, em alguns casos, utilize flex: 1; para definir um peso (explicarei melhor sobre isso mais para frente, porém no caso dessa página a utilização do flex: 1 não irá funcionar), a solução seria utilizar width absoluto, algo como (width: 200px ou 5rem ou 5em, tanto faz a unidade de medida) no mobile.
- Pode melhorar a escolha dos elementos no html (Semântica do html):
  - A div utilizada para a classe main-login poderia ser uma section ou o próprio header da página
- Utilizou o border-box no input, mas já havia definido que todos os elementos dentro do body já seria border-box;
- Não utilizou os breakpoints


## Vou reimplementar utilizando CSS e depois utilizando Boostrap + css puro
## Ver a pasta /correcoes