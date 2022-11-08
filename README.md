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

### DISTINCTCOUNT
<li>Conta o número de <strong>valores distintos/únicos</strong> (sem repetições) de uma coluna.</li>

### DISTINCTCOUNTNOBLANK
<li>Conta o número de <strong>valores distintos/únicos</strong> (sem repetições) de uma coluna, mas <strong>sem considerar os valores vazios/em branco</strong>.</li>

### COUNTROWS
<li>Conta o <strong>número de linhas na tabela especificada</strong> ou em uma tabela definida por uma expressão.</li>

## Funções Iteradoras
<li>Funções iteradoras permitem que você percorra a mesma expressão a cada linha de uma tabela e no final traga um único valor agregado.</li>

### SUMX

### COUNTX

### AVERAGEX

### RANKX

### CALCULATE
<li>Avalia uma expressão em um contexto de <strong>filtro</strong> modificado</li>
<li>A função CALCULATE funciona como a "SOMASE ou COUNT.SE" no Excel. A diferença é que aqui podemos criar medidas baseado em QUALQUER tipo de cálculo (não somente Soma, Contagem, etc), facilita pensar a função como "CALCULATESE"</li>
<li>Você calcula algo de acordo com o critério de filtro especificado.</li>

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

### DATEADD
<li>Retorna o resultado daquela medida correspondente a um <strong>período anterior</strong>.</li>

### SAMEPERIODLASTYEAR
<li>Retorna o resultado daquela medida correspondente a um <strong>ano anterior</strong>.</li>

### DATESYTD
<li>Retorna o <strong>resultado acumulado</strong> daquela medida até a presente data/momento.</li>

### DATESINPERIOD
<li>Retorna o <strong>resultado acumulado móvel</strong> de um <strong>período especificado</strong>.</li>

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

### CROSSFILTER
<li>Modifica a direção (<->) do filtro – é mais seguro do que deixar como "Both" e evita ambiguidade no modelo</li>
<li>Ao invés de utilizar relacionamentos bi-direcionais, utilize a CROSSFILTER para ativar a direção desejada em um caso específico.</li>

## Outras funções

### ALL
<li>Retorna todas as linhas de uma tabela, ou todos os valores de uma coluna, IGNORANDO qualquer filtro aplicado</li>
<li>Ao invés de adicionar um contexto de filtro, a função ALL remove os filtros daquele valor. Ela é muito utilizada quando você precisa de valores que não irão reagir as mudanças de filtro no dashboard (ex: <strong>% do total</strong>, onde o denominador deve permanecer um valor "fixo")</li>

### DIVIDE
<li>Função DIVIDE vs. operador (/)</li>
<li>Executa a divisão e retorna o resultado alternativo ou BLANK() na divisão por 0</li>
<li>A função DIVIDE foi criada para lidar automaticamente com casos de divisão por zero. Se um resultado alternativo não for passado e o denominador for zero ou ficar EM BRANCO, a função retornará "EM BRANCO". Quando um resultado alternativo é definido na função, ele será retornado, ao invés da palavra EM BRANCO (ou infinito)</li>

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

## Natureza dos dados

<img alt="Natureza dos Dados" title="Natureza dos Dados" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/natureza-dados.png" />

## Tipos de visualizações

Baseado na sua natureza, seguem algumas dicas para melhor visualização dos dados.

<img alt="Tipo de Variável" title="Tipo de Variável" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/tipo-variavel.png" />

Exemplo de como representar os dados quando se quer comparar duas variáveis baseado em sua natureza.

<img alt="Representação dos Dados" title="Representação dos Dados" src="https://github.com/robsonlopesjr/powerbi-guia/blob/master/imagens/representacao-dados.png" />