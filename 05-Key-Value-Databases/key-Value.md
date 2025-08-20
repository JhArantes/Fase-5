
# Key-Value DataBases

Claro! Esta aula aborda a tecnologia de bancos de dados NoSQL, com foco nos sistemas baseados em chave-valor. Aqui estão os principais pontos discutidos:

- **Natureza e características dos bancos chave-valor**: São simples, rápidos, flexíveis e escaláveis para grandes volumes de dados.
- **Tecnologias específicas**: Exemplos como Voldemort, Amazon Dynamo DB, Riak, Memcached e Redis são apresentados, destacando sua alta disponibilidade e desempenho.
- **Redis**: É um armazenamento de estruturas de dados em memória que suporta vários tipos de dados, como strings, hashes, listas, conjuntos e conjuntos ordenados. A aula inclui demonstrações de instalação, configuração e uso eficiente do Redis.
- **Aplicação prática**: Um caso de uso no desenvolvimento de um sistema IoT utilizando Redis com Golang para gerenciamento de dados de sensores.
- **Temas avançados**: O uso do Redis em operações com dados geoespaciais é abordado, relevante para aplicações de localização.
- **Atividades práticas**: Ao final, há atividades não avaliativas para reforçar o aprendizado e incentivar a exploração das capacidades do Redis.



Um armazenamento chave-valor é uma das formas mais simples de banco de dados NoSQL, baseado em pares chave → valor, semelhante a uma tabela hash.

Chave: string que identifica o dado.

Valor: qualquer tipo de informação associada.

Essa simplicidade garante velocidade, escalabilidade e flexibilidade, mas limita as consultas: só é possível buscar pelo valor conhecendo a chave. Não há suporte nativo a pesquisas complexas, esquemas ou relacionamentos.
      <div class="on-table-responsive">
        <table class="on-table on-table-primary">
          <thead>
            <tr>
              <th>Chave</th>
              <th>Valor</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>
                Nome
              </td>
              <td>
                Rita
              </td>
            </tr>
            <tr>
              <td>
                Idade
              </td>
              <td>
                22
              </td>
            </tr>
            <tr>
              <td>
                Telefone
              </td>
              <td>
                91234-5678, 91234-5679
              </td>
            </tr>
            <tr>
              <td>
                Endereço
              </td>
              <td>
                Avenida Lins de Vasconcelos, 1533
              </td>
            </tr>
            <tr>
              <td>
                Notas
              </td>
              <td>
                Biologia, 10, Matemática, 10
              </td>
            </tr>
          </tbody>
          <tfoot>
            <tr>
              <td colspan="Exemplos de chave-valor"></td>
            </tr>
          </tfoot>
        </table>
      </div>
Características

Schema less: não exige modelo de dados fixo.

Alto desempenho: suporta grandes volumes de leitura/gravação.

Baixo consumo de memória em relação a outros modelos.

Sem integridade referencial: não há chaves estrangeiras nem subconsultas.

Usos comuns

Gerenciamento de sessões em aplicativos web.

Perfis e preferências de usuários.

Recomendações e anúncios em tempo real.

Jogos online (controle de sessão de jogadores).

Carrinhos de compra em e-commerces.

Vantagens práticas

Empresas podem usar bancos chave-valor em períodos de pico (ex.: Black Friday, Natal), pois são mais fáceis de escalar e oferecem excelente custo-benefício.

Conclusão

O segredo desse modelo está na simplicidade e rapidez: a busca é direta, sem linguagens de consulta complexas. São ideais para cenários que exigem altíssimo desempenho e escalabilidade, embora com limitações em consultas avançadas e relacionamentos.