# Posicionamento de marcas de alvejante

##  🚀 Sobre
___

<br>Reprodução do exemplo de posiconamento de marcas no mercado de alvejantes, capítulo 2.1 do livro "Data Science, Marketing & Business" (https://datascience.insper.edu.br/datascience.pdf), em Python. </br>  
  
<br>A base de dados analisada é dividida em duas tabelas. A primeira tabela contém as respostas de 750 consumidores para 29 questões relacionadas à imagem de marcas de alvejantes. A segunda tabela contém as questões. Cada consumidor avaliou até quatro marcas e forneceu uma pontuação de 0 a 7 na escala de Likert.</br>

<br> Projeto pessoal com o objetivo de replicar o exercício proposto no livro com minha linguagem de programação favorita. </br>

## 💻 Instruções de Instalação
___

<br>Recomendo  bifurcar o repositório e cloná-lo localmente usando a função **git clone** no terminal. Instruções sobre como fazer isso podem ser acessadas [aqui](
https://docs.github.com/pt/github/getting-started-with-github/fork-a-repo).
</br>

``` bash
# Clonar repositório
git clone https://github.com/jluss0ll1/brand-positioning
```
Outra alternativa é clicar no botão verde "clone or download" neste repositório e então clicar em "Download ZIP". Em seguida, extrair o arquivo ZIP no local que você desejar editar ou executar o código.

## 🎫 Roteiro do Projeto

<br> Abri as duas tabelas no Python utilizando o Pandas e implementei o tratamento de dados. As pontuações de todos os consumidores para as 29 questões foram padronizadas e a contribuição de cada questão para a variabilidade dos dados foi obtida por Principal Component Analysis. Construí um "gráfico de cotovelo" para identificar os componentes que explicam a maior parte da variação de dados - os "drivers de valor" na linguagem do Marketing. Através do cálculo de "loading" (carga) dos componentes principais, descobri quais questões estavam relacionadas com cada driver, identificando assim os atributos que foram mais importantes na avaliação dos consumidores. Finalmente, criei um gráfico de linhas para organizar a pontuação de todas as marcas em cada um dos três principais drivers. </br>
