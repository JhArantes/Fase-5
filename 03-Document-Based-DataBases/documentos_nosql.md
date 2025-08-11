# Bancos de Dados Não Relacionais: Modelo de Documentos

## 📌 O que são?

Os **bancos de dados orientados a documentos** (ou *document-oriented databases*) são um tipo de banco de dados **NoSQL** projetado para armazenar, gerenciar e consultar **dados semiestruturados** no formato de **documentos**.  
Ao contrário dos bancos de dados relacionais, que usam **tabelas fixas com linhas e colunas**, os bancos de dados de documentos oferecem **flexibilidade no esquema**, permitindo que cada registro tenha campos e estruturas diferentes.

Esses documentos podem conter dados aninhados e hierárquicos, sendo mais próximos da forma como aplicações modernas manipulam dados.

**Principais formatos utilizados:**
- **JSON** (*JavaScript Object Notation*) — formato leve e legível por humanos.
- **BSON** (*Binary JSON*) — versão binária otimizada do JSON, usada por exemplo no MongoDB.
- **XML** (*Extensible Markup Language*) — formato estruturado e amplamente utilizado em integrações.

---

## 🗂 Estrutura e Flexibilidade

A característica central desse modelo é o **"schema-less"** (*esquema flexível*).  
Isso significa que documentos dentro da mesma **coleção** (equivalente a uma tabela) **não precisam ter exatamente o mesmo formato**.

**Exemplo de documentos (JSON):**

```json
// Documento 1
{
  "_id": "60c72b2f9f1b2c001f8e4e7e",
  "nome": "João Silva",
  "email": "joao.silva@email.com",
  "endereco": {
    "rua": "Rua das Flores, 123",
    "cidade": "São Paulo",
    "pais": "Brasil"
  },
  "pedidos": [
    { "id": "A123", "data": "2023-01-15", "total": 50.75 },
    { "id": "B456", "data": "2023-02-20", "total": 120.00 }
  ]
}
```

```json
// Documento 2 - Estrutura diferente
{
  "_id": "60c72b2f9f1b2c001f8e4e7f",
  "nome": "Maria Souza",
  "email": "maria.souza@email.com",
  "endereco": {
    "rua": "Avenida Brasil, 456",
    "cidade": "Rio de Janeiro"
  },
  "telefone": "55-21-98765-4321"
}
```

💡 No segundo documento, não existe a chave `"pais"`, mas há o campo `"telefone"`.  
Em bancos relacionais, isso exigiria **colunas nulas** ou **tabelas adicionais**, o que torna a modelagem mais complexa.

---

## ✅ Vantagens

- **Esquema flexível** — permite evoluir o modelo de dados sem migrações complexas.
- **Escalabilidade horizontal** — fácil distribuição dos documentos em múltiplos servidores.
- **Alto desempenho em consultas diretas** — leitura de um único documento traz todos os dados relacionados de uma vez.
- **Integração natural com linguagens de programação** — estrutura semelhante a objetos, facilitando o mapeamento.

---

## ⚠️ Desvantagens

- **Consultas complexas** — junções e relações entre coleções podem ser menos eficientes que no modelo relacional.
- **Falta de integridade referencial nativa** — não há chaves estrangeiras, exigindo controle via aplicação.
- **Atualizações parciais mais trabalhosas** — dependendo da implementação, atualizar campos específicos pode ser menos intuitivo.

---

## 🎯 Quando usar?

Bancos de dados de documentos são ideais para aplicações que exigem **flexibilidade de esquema** e **alta escalabilidade**, como:

- Sistemas de gerenciamento de conteúdo (**CMS**)
- Catálogos de produtos de **e-commerce**
- Perfis de usuários em redes sociais
- Dados de **Internet das Coisas (IoT)**
- Aplicações móveis e web que manipulam dados semiestruturados

---

## 🔹 Exemplos de Bancos de Dados de Documentos

- **MongoDB** *(o mais popular)*
- **Couchbase**
- **RethinkDB**
- **Azure Cosmos DB** *(suporta também outros modelos)*
