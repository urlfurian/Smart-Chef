# Smart-Chef

## Sobre o Projeto
**Projeto:** Smart-Chef
**Problema que resolve:** Impraticidade

## Integrantes
| Nome | GitHub |
|------|--------|
| [Matheus Augusto Furian Martins] | [@urlfurian] |
| [Miguel Franco Nardy] | [@MiguelNardy07] |
| [João Victor da Silva Santos] | [@JoãoVictor0102] |

## Arquitetura

```mermaid
flowchart TD

A[Usuario insere ingredientes - Formulario ou App] --> B[Armazenamento de dados - Banco ou Sheets]

B --> C[Processamento do estoque - validacao e organizacao]

C --> D[Consulta a API de receitas - TheMealDB]
D --> E[Filtragem de receitas compativeis]

E --> F[Envio para IA - Gemini ou OpenAI]
F --> G[IA sugere receita do dia + instrucoes]

G --> H[Formatacao da resposta]

H --> I[Notificacao ao usuario - Telegram, Email ou App]

C --> J[Verificacao de estoque baixo]
J --> I

C --> K[Deteccao de risco de gas]
K --> I
```
