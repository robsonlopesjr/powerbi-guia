## Funções de Agregação
<li>Úteis para agregar valores.
<li>Funcionam com colunas numéricas e agregam <strong>apenas UMA coluna por vez </strong>.

### SUM
<li>Adiciona todos os números de uma coluna</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/agregacao/sum/somar-qual-a-quantidade-de-itens-que-a-empresa-vendeu.pdf">Exemplo: Somar qual a quantidade de itens que a empresa vendeu.
</a></li>

### AVERAGE
<li>Retorna a medida aritmética de todos os números de uma coluna.</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/agregacao/average/qual-a-media-do-valor-dos-produtos.pdf">Exemplo: Qual a média do valor dos produtos.
</a></li>

### MAX
<li>Retorna o maior valor numérico de uma coluna ou entre duas expressões escalares.</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/agregacao/max/qual-o-valor-maximo-do-produto-vendido.pdf">Exemplo: Qual o valor máximo do produto vendido.
</a></li>
<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/agregacao/max/qual-a-ultima-data-existente-nos-dados.pdf">Exemplo: Qual a última data existente nos dados.
</a></li>

### MIN
<li>Retorna o menor valor numérico de uma coluna ou entre duas expressões escalares.</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/agregacao/min/qual-o-valor-minimo-do-produto-vendido.pdf">Exemplo: Qual o valor mínimo do produto vendido.
</a></li>

## Funções Estatísticas
<li>Diferenças entre as diferentes funções de contagem no Power BI.</li>

### COUNT
<li>Conta o número de células de uma coluna que contém <strong>números</strong>.</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/estatisticas/count/quantidade-de-pedidos-pelo-codigo-da-venda.pdf">Exemplo: Quantidade de pedidos pelo código da venda.
</a></li>

### DISTINCTCOUNT
<li>Conta o número de <strong>valores distintos/únicos</strong> (sem repetições) de uma coluna.</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/estatisticas/distinctcount/quantidade-de-pedidos-pelo-codigo-da-venda-de-forma-distinta.pdf">Exemplo: Quantidade de pedidos pelo código da venda de forma distinta.
</a></li>

### DISTINCTCOUNTNOBLANK
<li>Conta o número de <strong>valores distintos/únicos</strong> (sem repetições) de uma coluna, mas <strong>sem considerar os valores vazios/em branco</strong>.</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/estatisticas/distinctcountnoblank/quantidade-de-pedidos-pelo-codigo-da-venda-excluindo-valores-vazios.pdf">Exemplo: Quantidade de pedidos pelo código da venda (excluindo valores vazios).
</a></li>

### COUNTROWS
<li>Conta o <strong>número de linhas na tabela especificada</strong> ou em uma tabela definida por uma expressão.</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/estatisticas/countrows/quantidade-de-pedidos-pelo-codigo-da-venda-contando-todas-as-linhas-da-tabela.pdf">Exemplo: Quantidade de pedidos pelo código da venda (Contando a quantidade de linhas de uma tabela).
</a></li>

## Funções Iteradoras
<li>Funções iteradoras permitem que você percorra a mesma expressão a cada linha de uma tabela e no final traga um único valor agregado.</li>
<li>A grande vantagem de utilizar funções iteradoras é eliminar a necessidade de adicionar novas colunas calculadas no seu projeto.</li>

### SUMX

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/iteradoras/sumx/realizando-a-soma-de-valores-de-forma-acumulativa-entre-duas-colunas.pdf">Exemplo: Realizando a soma de valores de forma acumulativa entre duas colunas.
</a></li>

### COUNTX

### AVERAGEX

### RANKX
<li>Ideal para quando precisamos fazer um ranking de produtos, vendedores, clientes (e várias outras aplicações, de acordo com a situação de negócio).</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/iteradoras/rankx/criar-um-ranking-de-categorias-de-acordo-com-o-faturamento.pdf">Exemplo: Criar um ranking de categorias de acordo com o faturamento.
</a></li>

### CALCULATE
<li>Avalia uma expressão em um contexto de <strong>filtro</strong> modificado</li>
<li>A função CALCULATE funciona como a "SOMASE ou COUNTSE" no Excel. A diferença é que aqui podemos criar medidas baseado em QUALQUER tipo de cálculo (não somente Soma, Contagem, etc), facilita pensar a função como "CALCULATESE"</li>
<li>Você calcula algo de acordo com o critério de filtro especificado.</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/iteradoras/calculate/saber-o-faturamento-somente-de-uma-categoria.pdf">Exemplo: Saber o faturamento de somente uma categoria.
</a></li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/iteradoras/calculate/saber-o-faturamento-de-varias-categoria-exceto-algumas.pdf">Exemplo: Saber o faturamento de várias categoria, exceto alguma(s).
</a></li>

## Funções de Texto

### LEN
<li>Retorna o número de caracteres em uma cadeia de texto.</li>

### CONCATENATE
<li>Une duas cadeias de texto em uma única palavra.</li>

### LEFT/MID/RIGHT
<li>Retorna o número especificado de caracteres do início/meio/fim de uma cadeia de texto.</li>

### UPPER/LOWER/PROPER
<li>Converte todas as letras de um texto em maiúsculas (UPPER), minúsculas (LOWER) ou somente as primeiras letras como maiúsculas (PROPER).</li>

### SUBSTITUTE
<li>Substitui o texto original pelo novo texto em uma cadeia de texto.</li>

### VALUE
<li>Converte em número uma cadeia de texto que representa um número.</li>

## Funções de Inteligência de Tempo
<li><strong>Todas elas precisam da CALCULATE para funcionar</strong> e sempre que o argumento solicitado na fórmula for uma DATA, você deve referenciar somente a coluna Data da sua tabela dCalendário (mesmo que a comparação seja nível anual ou mensal, a coluna que você deve referenciar é a de DATA apenas.</li>

### DATEADD
<li>Retorna o resultado daquela medida correspondente a um <strong>período anterior</strong> (pode ser de mês, ano, dia ou trimestre - e você define o intervalo de comparação desejado).</li>
<li>Muito comum esse tipo de comparação para ver quanto evoluiu de um ano para o outro.</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/inteligencia_de_tempo/dateadd/saber-quanto-evoluiu-de-um-ano-para-o-outro.pdf">Exemplo: Saber quanto evoluiu de um ano para o outro.
</a></li>
<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/inteligencia_de_tempo/dateadd/saber-quanto-evoluiu-de-um-mes-para-o-outro.pdf">Exemplo: Saber quanto evoluiu de um mês para o outro.
</a></li>

### SAMEPERIODLASTYEAR
<li>Retorna o resultado daquela medida correspondente a um <strong>ANO anterior</strong> (somente ano).</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/inteligencia_de_tempo/sameperiodlastyear/saber-quanto-evoluiu-de-um-ano-para-o-outro.pdf">Exemplo: Saber quanto evoluiu de um ano para o outro.
</a></li>

### DATESYTD
<li>Retorna o <strong>resultado ACUMULADO</strong> daquela medida até a presente data/momento (Além de YTD (year-to-date) é possível também usar a DATESMTD (month-to-date) e DATESQTD (quarter-to-date).</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/inteligencia_de_tempo/datesytd/retorna-resultado-acumulado-ate-a-presente-data-atual.pdf">Exemplo: Retorna o resultado acumulado até a presente data.
</a></li>

### DATESINPERIOD
<li>Retorna o <strong>resultado acumulado MÓVEL</strong> de um <strong>período especificado</strong> (conhecido também como "running total").</li>

## Função FORMAT para datas

| Código | Descrição                    | Exemplo                                      |
| ------ | ---------------------------- | -------------------------------------------- |
| dddd   | nome completo do dia         | segunda-feira, terça-feira, quarta-feira ... |
| ddd    | primeiros 3 dígitos do dia   | seg, ter, qua, qui, sex ...                  |
| mmmm   | nome completo do mês         | janeiro, fevereiro, março, abril ...         |
| mmm    | primeiros 3 dígitos do mês   | jan, fev, mar, abr, mai, jun, jul ...        |
| mm     | núm. do mês com dois digitos | 01, 02, 03, 04, 05 ...                       |
| q      | quarter (= trimestre)        | 1, 2, 3, 4                                   |
| yyyy   | ano com quatro digitos       | 2018, 2019, 2020, 2021 ...                   |

## dCALENDARIO em DAX

### CALENDARAUTO
<li>Retorna uma tabela com apenas uma coluna chamada "Date" que contém um conjunto contíguo de datas. <strong>O intervalo de datas é calculado automaticamente</strong> com base nos dados no modelo.</li>

### CALENDAR
<li>Retorna uma tabela com apenas uma coluna chamada "Date" que contém um conjunto contínuo de datas. O intervalo de datas é da <strong>data de início especificada até a data de término especificada</strong>.</li>

## Fórmula pronta para criar uma tabela dimensão calendário dinâmica

1) Vá até a Guia Dados.
2) Clique em <strong>Nova Tabela</strong>.
3) Copie e cole o conteúdo abaixo na barra de fórmulas.
4) Altere a referência 'fVendas'[Data] para a coluna da tabela que contém a data desejada no seu modelo de dados.
5) Pressione <strong>Enter</strong>
6) Pronto! Sua tabela calendário dinâmica está criada e irá se atualizar conforme novas datas surgirem na tabela fato.

```
dCalendario Dinamica = 
VAR MinAno = YEAR(MIN('fVendas'[Data]))
VAR MaxAno = YEAR(MAX('fVendas'[Data]))
RETURN
ADDCOLUMNS(
    FILTER(
        CALENDARAUTO(),
        YEAR([Date]) >= MinAno &&
        YEAR([Date]) <= MaxAno
    ),
    "Ano", YEAR([Date]),
    "Num Trimestre", INT(FORMAT([Date], "q")),
    "Trimestre", "Q" & INT(FORMAT([Date],"q")),
    "Mês", MONTH([Date]),
    "Nome do mês", FORMAT([Date],"mmmm"),
    "Mês abrev", FORMAT([Date],"mmm"),
    "Semana do ano", WEEKNUM([Date])
)
```

## Funções Lógicas

### IF
<li>Verifica uma condição e retorna um valor quando é VERDADEIRO; caso contrário, retorna um segundo valor.</li>

### IFERROR
<li>Avalia uma expressão e retorna um valor especificado se a expressão retorna um erro; caso contrário, retorna o valor da própria expressão.</li>
<li>Ideal para combinar com outras funções</li>

### SWITCH
<li>Avalia uma expressão em relação a uma lista de valores e retorna uma das várias expressões de resultados possíveis.</li>
<li>Ideal para substituir o uso da função IF quando você tem uma situação com muitas condições (é posível combiná-la com a expressão TRUE (verdadeiro).</li>

## Funções de Relação

### RELATED
<li>Retorna um valor relacionado de outra tabela (traz valor do lado 1 – da tabela DIMENSÃO).</li>
<li>Essa função não realiza nenhuma operação matemática, apenas "abre a porta" para acessarmos colunas que estão em outra tabela relacionada no modelo.</li>

### RELATEDTABLE
<li>Retorna uma tabela relacionada, filtrada apenas com as linhas que possuem conexão (lado muitos - da tabela FATO).</li>
<li>Essa função normalmente é utilizada com outros agregadores, como COUNTROWS, SUMX, AVERAGEX, etc.</li>

### USERELATIONSHIP
<li>Força a ativação de um relacionamento inativo (---).</li>
<li>A função não retornará nenhum valor, apenas habilitará a relação indicada durante o cálculo.</li>
<li>Interessante para quando temos múltiplas tabelas de data no modelo (em tabelas diferentes) conectadas a uma única tabela dCalendário.</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/funcoes_de_relacao/userelationship/calcular-a-quantidade-de-documentos-entregues.pdf">Exemplo: Calcular a quantidade de documentos entregues.
</a></li>

### CROSSFILTER
<li>Modifica a direção (<->) do filtro – é mais seguro do que deixar como "Both" e evita ambiguidade no modelo</li>
<li>Ao invés de utilizar relacionamentos bi-direcionais, utilize a CROSSFILTER para ativar a direção desejada em um caso específico.</li>

## Outras funções

### ALL
<li>Retorna todas as linhas de uma tabela, ou todos os valores de uma coluna, IGNORANDO qualquer filtro aplicado</li>
<li>Ao invés de adicionar um contexto de filtro, a função ALL remove os filtros daquele valor. Ela é muito utilizada quando você precisa de valores que não irão reagir as mudanças de filtro no dashboard (ex: <strong>% do total</strong>, onde o denominador deve permanecer um valor "fixo")</li>
<li>Possibilita alterar o comportamento do filtro de um contexto no relatório.</li>
<li>A função ALL ignora quaisquer filtros aplicados (e considera a tabela como um todo, o valor total "fixo").</li>

<li><a href="https://github.com/robsonlopesjr/powerbi-guia/blob/master/iteradoras/rankx/criar-um-ranking-de-categorias-de-acordo-com-o-faturamento.pdf">Exemplo: Criar um ranking de categorias de acordo com o faturamento.
</a></li>

### DIVIDE
<li>Função DIVIDE vs. operador (/)</li>
<li>Executa a divisão e retorna o resultado alternativo ou BLANK() na divisão por 0</li>
<li>A função DIVIDE foi criada para lidar automaticamente com casos de divisão por zero. Se um resultado alternativo não for passado e o denominador for zero ou ficar EM BRANCO, a função retornará "EM BRANCO". Quando um resultado alternativo é definido na função, ele será retornado, ao invés da palavra EM BRANCO (ou infinito)</li>

## Natureza dos dados

<img alt="Natureza dos Dados" title="Natureza dos Dados" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/natureza-dados.png" />

## Tipos de visualizações

Baseado na sua natureza, seguem algumas dicas para melhor visualização dos dados.

<img alt="Tipo de Variável" title="Tipo de Variável" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/tipo-variavel.png" />

Exemplo de como representar os dados quando se quer comparar duas variáveis baseado em sua natureza.

<img alt="Representação dos Dados" title="Representação dos Dados" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/representacao-dados.png" />

## Gráficos mais usados no Power BI

### Variação no tempo
<li>Análises gráficas para mostrar a variação como uma determinada variável se comporta no tempo.</li>

<img alt="Gráficos de Variação no Tempo" title="Gráficos de Variação no Tempo" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/variacao-no-tempo.png" />

#### Colunas Empilhadas
Para criar o gráfico de colunas empilhadas no Power BI, devemos na primeira guia do Power BI, no menu à direita de Visualizações, procurar pelo ícone correspondente ao gráfico, e clicar. Arraste para onde quiser e dimensione de acordo com o que desejar.

Iremos procurar pela tabela de "Variação no Tempo", no menu à direita, onde teremos os nossos dados de interesse, e iremos inserir "Qtd. Vendas" como valores e "Data da Venda" como Eixo. Teremos, então, a seguinte visualização:

<img alt="Colunas Empilhadas" title="Colunas Empilhadas" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/colunas-empilhadas.png" />

<strong>O gráfico de colunas empilhadas nos traz uma visualização "quebrada"</strong> das vendas durante o ano, como se fizesse uma separação física entre os meses, o que não é o que queremos. <strong>O ideal</strong> para vermos a continuidade de vendas durante um período <strong>é uma visualização contínua</strong>, sem "quebras" ou separações.

O gráfico de <strong>linhas é melhor do que o de colunas empilhadas para dar essa sensação de continuidade</strong> dos dados.

#### Linhas
Para criar o gráfico de linhas no Power BI, lembre-se de clicar fora do gráfico de colunas empilhadas (na área em branco do nosso relatório) para ele não ser substituído ao criar o gráfico de linhas. Iremos no menu <strong>Visualizações</strong>, procurar pelo <strong>ícone</strong> correspondente ao gráfico, e <strong>clicar. Arraste para onde quiser</strong> e <strong>dimensione</strong> de acordo com o que desejar.

Iremos procurar pela tabela de "Variação no Tempo", no menu à direita, onde teremos os nossos dados de interesse, e iremos <strong>inserir "Qtd. Vendas" como valores e "Data da Venda" como Eixo</strong>, novamente. Teremos, então, a seguinte visualização:

<img alt="Linhas" title="Linhas" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/linhas.png" />

Temos também um gráfico muito parecido com o de linhas, que difere apenas pelo preenchimento da parte debaixo da linha (literalmente) até o eixo horizontal do gráfico com uma cor. Ele é como se fosse o gráfico de linhas com o preenchimento na parte debaixo da linha, o que dá um efeito visual interessante ao gráfico, que não parece ser mais "vazio".

#### Áreas
Para criar o gráfico de área no Power BI, lembre-se de clicar fora do gráfico de colunas empilhadas (na área em branco do nosso relatório) para ele não ser substituído ao criar o gráfico de área. Iremos no menu <strong>Visualizações</strong>, procurar pelo <strong>ícone</strong> correspondente ao gráfico, e <strong>clicar. Arraste para onde quiser</strong> e <strong>dimensione</strong> de acordo com o que desejar.

Iremos procurar pela tabela de "Variação no Tempo", no menu à direita, onde teremos os nossos dados de interesse, e iremos <strong>inserir "Qtd. Vendas" como valores e "Data da Venda" como Eixo</strong>, novamente. Teremos, então, a seguinte visualização:

<img alt="Área" title="Área" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/area.png" />

### Parte no todo
<li>Esses tipos de gráficos são comuns quando queremos representar quanto uma quantidade é representativa num total específico, ou seja, o quanto ela é importante no total em que ela está inserida.</li>
<li>A seguir veremos os gráficos mais comuns desse estilo para um exemplo de gastos em áreas diferentes e poderemos ver suas representatividades, sendo o somatório dos gastos individuais das áreas igual ao total de gastos.<li>

<img alt="Gráficos Parte no Todo" title="Gráficos Parte no Todo" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/parte-no-todo.png" />

#### Pizza
O primeiro tipo de gráfico que nos vêm à mente é o de pizza, onde teremos a distribuição das fatias da pizza de acordo com a representatividade de cada área (% do total) em relação ao total de gastos somados (100%). A maior representatividade implica numa fatia de tamanho maior, e uma representatividade menor implica numa fatia de tamanho menor na pizza.

Para criar esse tipo de gráfico devemos acessar a segunda aba de relatórios, a aba "2. Parte no todo", na parte inferior do Power BI. Lembre-se de clicar na área em branco do nosso relatório para continuar.

Então, iremos no menu <strong>Visualizações</strong>, procurar pelo <strong>ícone</strong> correspondente ao gráfico, e <strong>clicar. Arraste para onde quiser</strong> e <strong>dimensione</strong> de acordo com o que desejar.

Iremos procurar pela tabela de "Parte do Todo", no menu à direita, onde teremos os nossos dados de interesse, e iremos <strong>inserir "Gastos" como Legenda e "Total R$" como Valores</strong>, novamente. Teremos, então, o gráfico de pizza no Power BI:

<img alt="Pizza" title="Pizza" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/pizza.png" />

Quando temos muitas fatias de pizza, ou as partes (tamanho da fatia) são muito próximos, temos dificuldade de enxergar com clareza essa divisão.

#### Rosca
Para criar esse tipo de gráfico devemos acessar a segunda aba de relatórios, a aba "2. Parte no todo", na parte inferior do Power BI. Lembre-se de clicar na área em branco do nosso relatório para continuar.

Então, iremos no menu <strong>Visualizações</strong>, procurar pelo <strong>ícone</strong> correspondente ao gráfico, e <strong>clicar. Arraste para onde quiser</strong> e <strong>dimensione</strong> de acordo com o que desejar.

Iremos procurar pela tabela de "Parte do Todo", no menu à direita, onde teremos os nossos dados de interesse, e iremos <strong>inserir "Gastos" como Legenda e "Total R$" como Valores</strong>, novamente. Teremos, então, o gráfico de rosca no Power BI:

<img alt="Rosca" title="Rosca" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/rosca.png" />

#### Árvore
Para criar esse novo tipo de gráfico, também conhecido como treemap no Power BI, devemos acessar a segunda aba de relatórios, a "2. Parte no todo", na parte inferior do Power BI. Lembre-se de clicar na área em branco do nosso relatório para continuar.

Então, iremos no menu <strong>Visualizações</strong>, procurar pelo <strong>ícone</strong> correspondente ao gráfico, e <strong>clicar. Arraste para onde quiser</strong> e <strong>dimensione</strong> de acordo com o que desejar.

Iremos procurar pela tabela de "Parte do Todo", no menu à direita, onde teremos os nossos dados de interesse, e iremos <strong>inserir "Gastos" como Legenda e "Total R$" como Valores</strong>, novamente. Teremos, então, o gráfico de árvore no Power BI:

<img alt="Árvore" title="Árvore" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/arvore.png" />

Ele nos permite uma visão em "pizza quadrada" com as divisões de partes maiores preenchidas com as maiores participações dos gastos individuais nos totais, e ele consegue aproveitar melhor os rótulos de dados e a área do gráfico em si, em relação aos gráficos de Pizza e de Rosca.

#### Barras Empilhadas
Para criar o gráfico de barras empilhadas no Power BI nós devemos fazer o mesmo procedimento feito para os gráficos anteriores. Ou seja, clicar na área em branco do nosso relatório para continuar e escolher no menu Visualizações pelo ícone correspondente ao gráfico, e clicar. Arrastar para onde quiser e dimensione de acordo com o que desejar.

Iremos procurar pela tabela de "Parte do Todo", no menu à direita, onde teremos os nossos dados de interesse, e iremos <strong>inserir "Gastos" como Legenda e "Total R$" como Valores</strong>, novamente. Teremos, então, o gráfico de barras empilhadas:

<img alt="Barras Empilhadas" title="Barras Empilhadas" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/barras-empilhadas.png" />

Nesse tipo de gráfico não precisamos nos atentar ao todo para entender qual o maior, ele já ficará destacado numa barra maior que as outras na relação de gastos apresentada pelo gráfico.