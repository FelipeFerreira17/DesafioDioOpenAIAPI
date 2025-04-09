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

