# Tutorial de Saídas Estruturadas com LangChain
Este tutorial ensina como estruturar a saída de modelos de linguagem usando LangChain, permitindo obter respostas em formatos específicos, como JSON, ao invés de texto bruto. O exemplo usado demonstra como extrair informações de uma biografia, como nome, ano de nascimento, falecimento e trabalhos.

---
## Passo a Passo:

### 1. Instalação:
- Instale as bibliotecas necessárias: langchain, langchain-openai e google.colab.
### 2. Configuração:
- Importe as classes ChatOpenAI e PromptTemplate.
- Configure o modelo de linguagem (ex: gpt-4-mini) e defina a temperatura.
- Acesse sua chave de API da OpenAI.
### 3. Criando o Prompt Template:
- Utilize PromptTemplate para criar um prompt que instrui o modelo a retornar as informações desejadas em formato JSON.
### 4. Criando a Cadeia LangChain:
- Utilize a classe chain para conectar o PromptTemplate ao modelo de linguagem.
### 5. Executando a Cadeia:
- Utilize o método invoke da cadeia, passando a biografia como entrada, para obter a resposta do modelo.
### 6. Extraindo a Resposta:
- Utilize StrOutputParser para extrair a resposta em formato JSON.
### 7. Validação e Estruturação com Pydantic:
- Importe BaseModel e Field da biblioteca pydantic.
- Crie uma classe que herda de BaseModel e defina os campos desejados, especificando seus tipos e descrições.
### 8. Criando o Modelo com Saída Estruturada:
- Utilize a função with_structured_output para criar uma versão do modelo de linguagem que retorna a saída estruturada de acordo com a classe criada.
### 9. Utilizando o Modelo Estruturado:
- Utilize o método invoke do modelo estruturado, passando a biografia como entrada.
### 10. Acessando os Dados:
- Acesse os dados da resposta usando a notação de ponto na resposta estruturada.
### 11. Ajustando o Prompt:
- Ajuste o prompt para obter resultados mais precisos.

---

## Link para o vídeo: 
(link do vídeo)[https://www.youtube.com/watch?v=CJLbck4tLkc&list=WL&index=2]
