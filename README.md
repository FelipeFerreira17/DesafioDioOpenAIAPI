# Desafio DIO OpenAI API e Semantic Kernel.

## API DO Azure OpenAi
Com a API do Azure OpenAI podemos integrar modelos de Inteligência Artificial em sites, sistemas ou aplicativos.
Pode ser usada para:
* Geração de texto
* Compreenção de linguagem
* Tradução de textos
* Respostas automatizadas
* Análise de sentimentos.

Para usar a API, devemos ter uma conta no Azure, obter uma chave de API e usar essa chave para fazer chamadas para os endpoints da API
Tendo a chave de API, pode-se programar, como por exemplo no código abaixo:

```
import openai

# Defina a chave da API do Azure OpenAI
openai.api_key = 'sua-chave-de-api'

# Se você está usando um endpoint específico do Azure OpenAI, configure isso também
openai.api_base = "https://<seu-endpoint>.openai.azure.com/"

# Exemplo de requisição para o modelo GPT-4
response = openai.Completion.create(
  engine="gpt-4",  # Pode ser 'gpt-3.5-turbo', 'gpt-4', etc.
  prompt="Qual é a capital do Brasil?",
  max_tokens=50
)

# Exibir a resposta
print(response.choices[0].text.strip())
```
Esse foi um exemplo de código que podemos usar para API do Azure OpenAI.

# Semantic Kernel
Semantic Kernel é uma ferramenta que permite integrar inteligência Artificial em fluxos de trabalho e aplicações,conbinando IA generativa com tecnicas de planejamento, memória e execução de tarefas.
## Principais características do Semantic Kernel
* Orquestração de Ações
* Personalização
* Integração com Diferentes Fontes de Dados
* Escalabilidade
* Open Source

Resumindo, Semantic Kernel é uma ferramenta poderosa para desenvolvedores que desejam orquestrar e integrar modelos de linguagem avançados de forma inteligente e personalizada. Ele facilita a criação de fluxos de trabalho complexos, permitindo que você use IA de maneira mais estruturada e funcional, em vez de apenas enviar e receber texto de forma simples.
