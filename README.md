# IA Generativa com Copilot (Microsoft) e OpenAI

Este documento fornece uma visão geral dos recursos de Inteligência Artificial Generativa disponíveis nas plataformas **Microsoft Copilot** e **OpenAI**, incluindo seus objetivos, aplicações e um passo a passo para começar a usar.

---

## 🧠 Visão Geral

### Copilot (Microsoft 365)
O **Copilot** integra modelos de linguagem da OpenAI (como o GPT-4) nas ferramentas do Microsoft 365, como Word, Excel, PowerPoint, Outlook e Teams.

### OpenAI
A **OpenAI** oferece APIs e ferramentas como **ChatGPT**, **DALL·E**, **Whisper** e modelos de linguagem para integrar IA generativa em diferentes soluções.

---

## 🎯 Objetivos Principais

- Aumentar produtividade com automação de tarefas.
- Facilitar a criação de conteúdos (textos, apresentações, imagens).
- Ajudar na análise e interpretação de dados.
- Suportar comunicação eficiente e personalizada.
- Promover inovação com prototipação rápida.
- Apoiar aprendizado e desenvolvimento contínuo.

---

## 🧩 Recursos Disponíveis

### Com Microsoft Copilot:
| Aplicativo | Recursos com IA |
|------------|------------------|
| Word       | Gerar, revisar e resumir textos |
| Excel      | Criar fórmulas, analisar dados, gerar gráficos |
| PowerPoint | Criar apresentações automaticamente |
| Outlook    | Escrever/resumir e-mails, gerar respostas |
| Teams      | Resumo de reuniões, geração de tarefas |

### Com OpenAI:
- **ChatGPT**: assistente de escrita, tutor, programador virtual.
- **DALL·E**: geração e edição de imagens por texto.
- **Whisper**: transcrição e tradução de áudios.
- **API OpenAI**: integração de IA em apps, sites e bots.

---

## 🚀 Passo a Passo para Usar

### 1. Usando o Microsoft Copilot
> Requer assinatura do Microsoft 365 com Copilot habilitado

1. Acesse um app do Office (Word, Excel, etc.).
2. Clique no ícone do **Copilot**.
3. Digite um comando como:
   - "Resuma este documento"
   - "Crie uma apresentação com base nesse texto"
   - "Sugira uma fórmula para calcular lucro líquido"
4. Revise e edite conforme necessário.

### 2. Usando o ChatGPT (OpenAI)
1. Acesse: [https://chat.openai.com](https://chat.openai.com)
2. Crie uma conta (ou entre com sua conta OpenAI).
3. Digite uma pergunta ou solicitação no chat.
4. Use ferramentas avançadas se disponíveis:
   - Geração de imagens (DALL·E)
   - Análise de arquivos (PDFs, planilhas)
   - Navegação na web (ChatGPT Plus)

### 3. Usando a API da OpenAI
> Para desenvolvedores ou empresas

1. Crie uma conta em: [https://platform.openai.com](https://platform.openai.com)
2. Gere uma chave de API.
3. Escolha o modelo (GPT-4, DALL·E, Whisper).
4. Envie solicitações via código:
```python
import openai

openai.api_key = "SUA_API_KEY"

response = openai.ChatCompletion.create(
  model="gpt-4",
  messages=[{"role": "user", "content": "Explique a teoria da relatividade"}]
)

print(response.choices[0].message['content'])
