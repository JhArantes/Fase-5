
# Teste de Hipoteses

<p>
        Além de conhecer as medidas descritivas, entender conceitos importantes de probabilidade e aplicar métodos de amostragem para obter os dados, torna-se importante realizar perguntas aos dados. Essas perguntas podem ser transformadas em afirmações, e, deste modo, aplicar técnicas de inferência estatística para validar essas afirmações.
      </p>


- O que é uma hipótese?
    - É uma Afirmação sobre um questionamento levantado pela empresa
       
- Por que criamos hipóteses?
    - Porque precisamos transformar um Questionamento em uma Afirmação
           
          
- Quais os riscos relacionados quando se busca testar uma hipótese?
    - Erro de interpretação: acreditar que uma relação é causal quando é apenas uma correlação.

    - Viés nos dados: se a amostra não representa bem a população, os resultados podem ser enganosos.

    - Erros estatísticos:

        - Erro Tipo I (falso positivo) – rejeitar uma hipótese verdadeira.

        - Erro Tipo II (falso negativo) – não rejeitar uma hipótese falsa.

    - Tomada de decisão equivocada: se a hipótese for mal formulada ou mal testada, pode levar a estratégias erradas.
           
- Caso exista um erro no processo, quais as consequências?
    - No nível analítico: conclusões estatísticas incorretas, relatórios imprecisos e análises inconsistentes.

    - No nível empresarial:

        - Investimentos em estratégias ineficientes.

        - Perda de tempo e recursos.

        - Risco de perda de competitividade no mercado.

    - No nível estratégico: perda de confiança na área de dados e dificuldade em embasar decisões futuras.

### Passos

1. Fixar Hipóteses H0 e H1 -> Nula e alternativa

2. Definir Estimador -> Média, Variância, Mediana

3. Nível de Confiança -> 90% -> 99%

4. Calcular Teste -> Teste t / f

5. Responnder Hipótese (Rejeitar Hipotese Nula / Não Rejeitar Hipótese Nula)


- Teste AB


<p>
        Realizar questionamentos sobre comportamento dos clientes, operações e resultados financeiros são tarefas comuns no ambiente de negócios. Do ponto de vista científico, perguntas são respondidas, não testadas. Diante disso, para testarmos perguntas de negócios, torna-se necessário transformá-las em afirmações e assim possibilitar o teste.
      </p>

<p>
        Dessa forma, podemos definir o conceito de teste de hipótese como:
      </p>
<p>
          Metodologia que permite verificar se os dados da amostra trazem evidências para rejeitar ou não rejeitar a hipótese proposta.
        </p>

## Procedimentos e tipos de Testes

<p>
        Os procedimentos para testes de hipótese mais adotados foram propostos por Fisher, Neyman e Pearson, conforme apresentam Huberty (1993), Biau <i>et. al.</i> (2010) e Perezgonzales (2015). No caso de Fisher, o foco é obter o nível descritivo, quanto ao método de Neyman e Pearson, o mais importante é estabelecer o valor crítico. No quadro “Procedimentos para realizar um teste de hipótese” apresentamos ambas as metodologias.
      </p>

<table class="on-table on-table-primary">
          <thead>
            <tr>
              <th>Etapas</th>
              <th>Fisher</th>
              <th>Neyman-Pearson</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>
                1
              </td>
              <td>
                Definir a hipótese nula.
              </td>
              <td>
                Fixar a hipótese nula e a hipótese alternativa.
              </td>
            </tr>
            <tr>
              <td>
                2
              </td>
              <td>
                Definir o teste e a distribuição de probabilidade.
              </td>
              <td>
                Definir qual estimador será utilizado (média, variância).
              </td>
            </tr>
            <tr>
              <td>
                3
              </td>
              <td>
                Obter os dados e estimar a estatística de teste.
              </td>
              <td>
                Fixar o nível de confiança (90%, 95%, 99%) para definir o valor crítico.
              </td>
            </tr>
            <tr>
              <td>
                4
              </td>
              <td>
                Definir o nível descritivo.
              </td>
              <td>
                Utilizar os dados da amostra obtida para calcular o valor da estatística teste.
              </td>
            </tr>
            <tr>
              <td>
                5
              </td>
              <td>
                Rejeitar a hipótese nula se o nível descritivo for menor que o valor definido na etapa 4.
              </td>
              <td>
                Rejeitar a hipótese nula se o valor da estatística de teste for maior que o valor definido na etapa 3.
              </td>
            </tr>
          </tbody>
</table>

<table class="on-table on-table-primary">
          <thead>
            <tr>
              <th>Teste</th>
              <th>Hipótese Nula</th>
              <th>Hipótese Alternativa</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>
                t
              </td>
              <td>
                <b>ℎ₀: μA = μB</b>
              </td>
              <td>
                <b>ℎ: μA ≠ μB </b>
              </td>
            </tr>
            <tr>
              <td>
                F
              </td>
              <td>
                <b>ℎ₀: μ₁ = μ₂ = ... = μK </b>
              </td>
              <td>
                <b>ℎ: μ₁ ≠ μ₂ ≠ ... ≠ μK</b>
              </td>
            </tr>
            <tr>
              <td>
                Qui-Quadrado
              </td>
              <td>
                <b>ℎ₀: NÃO Existe associação entre A e B</b>
              </td>
              <td>
                <b>ℎ: Existe associação entre A e B</b>
              </td>
            </tr>
            <tr>
              <td>
                Correlação
              </td>
              <td>
                <b>ℎ₀:ρ  = 0</b>
              </td>
              <td>
                <b>ℎ₀:β = 0</b>
              </td>
            </tr>
            <tr>
              <td>
                Regressão
              </td>
              <td>
                <b>ℎ₀:ρ ≠ 0</b>
              </td>
              <td>
                <b>ℎ₀:β ≠ 0 </b>
              </td>
            </tr>
          </tbody>
</table>

<p>
        Em relação ao teste t, a hipótese básica é verificar se existem diferenças quanto à média quando comparamos dois grupos. No teste F, testamos as diferenças de médias para mais de 2 grupos. O teste de Qui-Quadrado analisa a associação entre duas variáveis categóricas, enquanto no teste de correlação analisa-se a correlação (ρ) entre duas variáveis numéricas. Por fim, o teste de regressão verifica se uma variável x influencia uma variável y, o grau de influência é observado pelo valor de β.
      </p>


### Consequências do Erro

Especialistas na área de Analytics consideram dois tipos de riscos:
    
- Rejeitar a hipótese nula, quando não deveria rejeitar.
- Não rejeitar a nula, quando deveria rejeitar.
         
<table class="on-table on-table-primary">
          <thead>
            <tr>
              <th>Erros</th>
              <th>Rejeitar H0</th>
              <th>Não rejeitar H0</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>
                H0 Verdade
              </td>
              <td>
                Erro Tipo I (α)
              </td>
              <td>
                Ok
              </td>
            </tr>
            <tr>
              <td>
                H0 Falso
              </td>
              <td>
                Ok
              </td>
              <td>
                Erro Tipo II (ρ)
              </td>
            </tr>
          </tbody>
</table>


## Principais funções no Python

<table class="on-table on-table-primary">
          <thead>
            <tr>
              <th>Módulos</th>
              <th>Funções</th>
              <th>Aplicação</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>
                <i>Numpy</i>
              </td>
              <td>
                Várias funções serão utilizadas
              </td>
              <td>
                Análise numérica
              </td>
            </tr>
            <tr>
              <td>
                <i>Pandas</i>
              </td>
              <td>
                Várias funções serão utilizadas
              </td>
              <td>
                Leitura e tratamento de dados
              </td>
            </tr>
            <tr>
              <td>
                <i>Matplotlib</i>
              </td>
              <td>
                Várias funções serão utilizadas
              </td>
              <td>
                Análise gráfica
              </td>
            </tr>
            <tr>
              <td>
                <i>Seaborn</i>
              </td>
              <td>
                Várias funções serão utilizadas
              </td>
              <td>
                Análise gráfica
              </td>
            </tr>
            <tr>
              <td rowspan="2"><i>scipy.stats</i>
              </td>
              <td>
                <i>ttest_ind</i>
              </td>
              <td>
                Teste t
              </td>
            </tr>
            <tr>
              <td>
                <i>f_oneway</i>
              </td>
              <td>
                Teste F
              </td>
            </tr>
            <tr>
              <td rowspan="2"><i>pingouin</i>
              </td>
              <td>
                <i>ttest</i>
              </td>
              <td>
                Teste t mais detalhado
              </td>
            </tr>
            <tr>
              <td>
                <i>anova</i>
              </td>
              <td>
                Teste F mais detalhado
              </td>
            </tr>
          </tbody>
</table>

## Dados e exemplos

