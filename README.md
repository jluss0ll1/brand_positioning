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

## 💾 Ferramentas utilizadas

* Python
* Jupyter Notebook
* Pandas
* scikit-learn
* Principal Component Analysis

## 🎫 Visão Geral do Projeto

<br> As 29 perguntas envolvem todo tipo de características sobre alvejantes (intensidade da limpeza, suavidade do aroma, etc.), a proposta do projeto é identificar nas questões quais podem ser considerados os "drivers de valor" - os atributos que direcionam a demanda dos consumidores. </br> 

<br> Para isso, abri as duas tabelas no Python utilizando o Pandas e implementei o tratamento de dados. As pontuações de todos os consumidores para as 29 questões foram padronizadas e a contribuição de cada questão para a variabilidade dos dados foi obtida através de Principal Component Analysis (PCA). Construí um "gráfico de cotovelo" para identificar os componentes que explicam a maior parte da variação de dados - os "drivers de valor" na linguagem do Marketing. Pelo gráfico é possível observar que três componentes - ainda não plenamente identificados - explicavam 59,42% dos dados.</br> 

![image](https://user-images.githubusercontent.com/65292945/127380406-9b9f2b3b-7019-4496-9422-4b77814f3e8a.png)

<br> Através do cálculo de "loading" (carga) dos componentes principais, descobri quais questões estavam relacionadas com cada driver, identificando assim os atributos que foram mais importantes na avaliação dos consumidores. Finalmente, criei um gráfico de linhas para organizar a pontuação de todas as marcas em cada um dos três atributos identificados. </br>

![image](https://user-images.githubusercontent.com/65292945/127380495-677638e4-3079-46a5-a852-980b07c58067.png)

<br> Pode-se observar, por exemplo, que a marca de alvejantes AbraxF obteve o melhor desempenho no quesito "Limpeza", enquanto a marca RiUtil obteve a melhor performance em "Intensidade" e "Suavidade". </br>

<br> A informação sobre o posicionamento das marcas e a obtenção de drivers serve como um guia para equipes publicitárias enfatizarem os pontos fortes de sua própria marca ou comparar o desempenho dos seus produtos com os concorrentes. Pode também guiar a equipe responsável pelo desenvolvimento do produto em um redesign para melhorar seu desempenho nos aspectos que obteve baixa pontuação.  </br> 
