# ⚡ Elastic Stack (ELK)

**Elastic Stack** – também chamado de **ELK** – é o conjunto de três poderosas ferramentas *open source* para **ingestão, tratamento, armazenamento e análise de dados**:  

- **🔍 Elasticsearch** → Mecanismo de busca e análise de dados distribuído.  
- **🔄 Logstash** → Pipeline de ingestão e processamento de dados.  
- **📊 Kibana** → Visualização interativa com gráficos e dashboards.  

Além disso, há os **📦 Beats**, conectores leves que enviam dados para o Elasticsearch.  

---

## 🔍 Elasticsearch

Banco de dados orientado a documentos, baseado no Apache Lucene, lançado em 2010.  
Permite armazenar e analisar dados **textuais, numéricos, geoespaciais, estruturados e não estruturados** com alta velocidade e escalabilidade.  

✨ **Destaques**:  
- REST APIs simples  
- Arquitetura distribuída  
- Alta performance e escalabilidade  
- Integração com **Logstash**, **Kibana** e **Beats**

---

## 🔄 Logstash

Ferramenta *open source* de **ingestão e processamento de dados**.  
📥 Coleta dados de diversas fontes (logs, eventos, JSON, CSV, etc.)  
🛠️ Enriquecimento e transformação de dados antes de enviá-los ao destino.  
📤 Envio para Elasticsearch, bancos de dados, nuvem ou sistemas de análise.  

💡 No **ELK Stack**, o **Logstash** recebe dados, transforma, normaliza e indexa no **Elasticsearch**, enquanto o **Kibana** exibe dashboards e relatórios visuais.

---

## 📦 Beats

Pequenos agentes leves que enviam dados diretamente para o Elasticsearch ou Logstash, funcionando como **coletores na borda** (*edge machines*).  

Exemplos:  
- **🌐 Packetbeat** → Monitoramento de tráfego de rede em tempo real.  
- **📜 Filebeat** → Coleta de arquivos de log.  
- **📈 Metricbeat** → Métricas do sistema e serviços.  
- **🔒 Auditbeat** → Dados de auditoria de segurança.  
- **🖥 Winlogbeat** → Eventos do Windows.  

Mais de **160 Beats criados pela comunidade** ampliam as possibilidades para todos os tipos de dados operacionais.
