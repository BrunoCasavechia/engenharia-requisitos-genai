# Engenharia de Requisitos com GenAI — Sistema de Gestão de Eventos (Eventus)

Atividade prática da Unidade III do curso Engenharia de Requisitos com Inteligência Artificial Generativa (AKCIT/UFG). Análise e especificação de requisitos a partir do documento de elicitação do sistema Eventus, fornecido no material de estudos da unidade.

## Estrutura do repositório

```
engenharia-requisitos-genai/
├── README.md
├── analise/
│   ├── requisitos-funcionais.md
│   ├── requisitos-nao-funcionais.md
│   ├── regras-de-negocio.md
│   └── duvidas-e-lacunas.md
└── especificacao/
    ├── historias-de-usuario.md
    ├── casos-de-uso.md
    └── criterios-de-aceitacao.md
```

## Artefatos de especificação escolhidos

Foram escolhidos **histórias de usuário**, **casos de uso** e **critérios de aceitação**. A combinação foi considerada mais adequada porque o Eventus tem cinco perfis de stakeholders com necessidades distintas (participante, organizador, equipe financeira, palestrante, equipe de TI) e fluxos que envolvem múltiplas condições e exceções — inscrição com pagamento condicional, cancelamento com regras variáveis, lista de espera. As histórias de usuário registram o valor de negócio na voz de quem pediu a funcionalidade; os casos de uso detalham os fluxos mais complexos com suas exceções; os critérios de aceitação tornam cada comportamento verificável e prontos para virar teste.

Protótipos não foram produzidos nesta etapa porque várias lacunas de interface (ex.: como funciona a lista de espera, quais dados o palestrante vê) ainda não foram esclarecidas — prototipar antes disso arriscaria fixar decisões de tela que ainda não têm requisito por trás.

## Como a IA Generativa apoiou a atividade

Utilizei o Claude como apoio em cada etapa: primeiro para organizar o texto bruto do documento de elicitação em requisitos funcionais, regras de negócio e lacunas; depois para sugerir quais artefatos de especificação seriam mais adequados dado o perfil do projeto; e por fim para gerar as primeiras versões das histórias de usuário, casos de uso e critérios de aceitação a partir dos requisitos já organizados.

## Sugestões aceitas, modificadas e descartadas

**Aceitas:** a separação inicial dos requisitos em funcionais, regras de negócio e lacunas; a estrutura geral de histórias de usuário + casos de uso + critérios de aceitação; o formato Dado-Quando-Então para os critérios.

**Modificadas:** os requisitos não funcionais sugeridos pela IA foram reclassificados como "candidatos, a validar" em vez de requisitos definitivos, porque o documento de elicitação afirma explicitamente que nenhum RNF foi levantado nas entrevistas — apresentá-los como certos seria inventar informação que não existe na fonte.

**Descartadas:** a IA sugeriu, em alguns pontos, preencher lacunas como o critério de reembolso e o funcionamento da lista de espera com respostas plausíveis. Optei por não aceitar essas suposições e manter as lacunas explícitas no documento `duvidas-e-lacunas.md`, já que são pontos que dependem de validação direta com os stakeholders do projeto e não deveriam ser decididos unilateralmente.

## Cuidados observados durante o uso da IA

A IA foi útil para acelerar a organização do material bruto e sugerir uma primeira versão dos artefatos, mas teve tendência a preencher lacunas com respostas coerentes, porém não confirmadas por ninguém — algo arriscado numa etapa de especificação, onde o objetivo é representar fielmente o que foi levantado, não completar buracos com suposições. Por isso, cada lacuna do documento original foi mantida como lacuna, e cada sugestão de RNF foi rotulada como candidata em vez de definitiva. A validação humana continuou sendo essencial para garantir que a especificação refletisse exatamente o que estava (e o que não estava) no documento de elicitação.
