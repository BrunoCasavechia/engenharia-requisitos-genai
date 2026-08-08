# Critérios de Aceitação — Sistema de Gestão de Eventos (Eventus)

Critérios no formato Dado–Quando–Então para as histórias de usuário mais críticas.

## HU02 — Inscrever-se em evento

| Dado | Quando | Então |
|---|---|---|
| O evento está com inscrições abertas e possui vagas disponíveis | O participante se inscreve | O sistema registra a inscrição e envia um comprovante |
| O evento está com inscrições abertas mas sem vagas disponíveis | O participante tenta se inscrever | O sistema oferece a opção de entrar na lista de espera |
| O evento é pago | O participante se inscreve | A inscrição só é confirmada após a confirmação do pagamento pela equipe financeira |

## HU04 — Cancelar inscrição

| Dado | Quando | Então |
|---|---|---|
| O participante possui inscrição ativa em evento que permite cancelamento | Solicita o cancelamento | O sistema efetiva o cancelamento sem exigir contato com a organização |
| O participante possui inscrição ativa em evento que não permite cancelamento | Solicita o cancelamento | O sistema informa que o cancelamento não é permitido para esse evento |

## HU08 — Acompanhar inscritos em tempo real

| Dado | Quando | Então |
|---|---|---|
| O organizador está visualizando o painel de um evento | Uma nova inscrição é registrada | O número de inscritos exibido é atualizado sem necessidade de recarregar a página manualmente |

## HU10 — Consultar participantes inscritos (palestrante)

| Dado | Quando | Então |
|---|---|---|
| O palestrante está autenticado e possui atividades vinculadas | Acessa a lista de participantes de uma atividade | O sistema exibe os participantes inscritos naquela atividade específica |
| O palestrante tenta acessar participantes de uma atividade que não é sua | — | O sistema nega o acesso |

---
*Nota: critérios gerados com apoio de IA a partir das histórias de usuário e revisados para ficarem objetivamente verificáveis, conforme a característica "verificável" da ISO/IEC/IEEE 29148.*
