# automacao-comercial-n8n

Pipeline de qualificação de leads B2B com n8n — integração com CRM e IA aplicada a operações comerciais.

## Problema que resolve

Operações B2B perdem leads por falta de processo automatizado: entrada manual, qualificação subjetiva, follow-up baseado em memória do vendedor.

Este workflow automatiza:
- Captura de leads de múltiplas fontes
- - Enriquecimento e qualificação por score
  - - Roteamento automático para CRM
    - - Gatilho de sequência de follow-up
      -
      - ## Fluxo
      -
      - ```
        Lead entra (webhook/formulário/LinkedIn)
        → n8n processa e enriquece dados
        → Claude API classifica: quente / morno / frio
        → Score calculado por critérios do ICP
        → HubSpot atualizado com etapa e próxima ação
        → Vendedor notificado com contexto completo
        ```

        ## Stack

        - **n8n** — orquestração do workflow
        - - **Claude API** — classificação e análise de perfil
          - - **HubSpot API** — CRM de destino
            - - **Webhook** — entrada de dados
              -
              - ## Estrutura
              -
              - ```
                automacao-comercial-n8n/
                ├── README.md
                ├── LICENSE
                ├── .gitignore
                ├── /docs
                │   ├── arquitetura.md
                │   └── decisoes.md
                ├── /workflows
                │   └── pipeline.json
                ├── /screenshots
                │   └── fluxo.png
                └── /examples
                    └── payload.json
                ```

                ## Resultado esperado

                - Redução de 80%+ no tempo de qualificação manual
                - - Dados completos no CRM desde o primeiro contato
                  - - Vendedor focado em fechar, não em preencher
                    -
                    - ## Contato
                    -
                    - Consultoria em automação B2B: [linkedin.com/in/gabriel-bianco-](https://linkedin.com/in/gabriel-bianco-)# automacao-comercial-n8n
