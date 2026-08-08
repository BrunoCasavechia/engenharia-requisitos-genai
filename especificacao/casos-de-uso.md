# Casos de Uso — Sistema de Gestão de Eventos (Eventus)

Foram escolhidos os três fluxos mais complexos do sistema para detalhamento em casos de uso, já que envolvem múltiplas condições, atores e exceções — algo que uma história de usuário sozinha não descreve bem.

## UC01 — Inscrever-se em Evento

| Campo | Descrição |
|---|---|
| Nome | Inscrever-se em Evento |
| Objetivo | Permitir que o participante se inscreva em um evento disponível |
| Ator principal | Participante |
| Atores secundários | Equipe Financeira (para eventos pagos) |
| Pré-condição | O evento está com inscrições abertas |
| Fluxo principal | 1. O participante seleciona um evento na lista.<br>2. O sistema verifica disponibilidade de vagas.<br>3. Caso o evento seja pago, o sistema encaminha para confirmação de pagamento.<br>4. A equipe financeira confirma o pagamento.<br>5. O sistema registra a inscrição.<br>6. O sistema envia comprovante ao participante. |
| Fluxo alternativo 1 | Evento sem vagas disponíveis → o sistema oferece entrada na lista de espera (ver RN05; regras de funcionamento da lista ainda não definidas — lacuna 3). |
| Fluxo alternativo 2 | Participante tenta se inscrever em atividade com horário conflitante com outra inscrição já confirmada → tratamento não definido (lacuna 7); sugerido bloquear a inscrição até validação com stakeholders. |
| Pós-condição | Inscrição registrada e comprovante enviado ao participante. |

## UC02 — Cancelar Inscrição

| Campo | Descrição |
|---|---|
| Nome | Cancelar Inscrição |
| Objetivo | Permitir que o participante cancele sua própria inscrição sem contato manual com a organização |
| Ator principal | Participante |
| Pré-condição | O participante possui uma inscrição ativa em um evento que permite cancelamento (RN03) |
| Fluxo principal | 1. O participante acessa suas inscrições.<br>2. Seleciona o evento a cancelar.<br>3. O sistema verifica se o evento permite cancelamento.<br>4. O sistema verifica se o participante tem direito a reembolso (critério não definido — lacuna 2).<br>5. O sistema efetiva o cancelamento. |
| Fluxo alternativo | Evento não permite cancelamento → o sistema informa o participante e orienta contato com a organização. |
| Pós-condição | Inscrição cancelada; vaga liberada para lista de espera (se houver). |

## UC03 — Consultar Participantes Inscritos (Palestrante)

| Campo | Descrição |
|---|---|
| Nome | Consultar Participantes Inscritos |
| Objetivo | Permitir que o palestrante visualize quem está inscrito em suas atividades |
| Ator principal | Palestrante |
| Pré-condição | O palestrante está autenticado e possui atividades vinculadas a ele |
| Fluxo principal | 1. O palestrante acessa suas atividades.<br>2. Seleciona uma atividade.<br>3. O sistema exibe a lista de participantes inscritos. |
| Fluxo alternativo | Nenhum participante inscrito ainda → o sistema informa lista vazia. |
| Pós-condição | Lista de participantes exibida ao palestrante. |
| Observação | Quais campos exatos dos participantes ficam visíveis ao palestrante não foi definido no material de elicitação (lacuna 8) — sugestão inicial: nome e organização/instituição, sem dados de contato ou pagamento. |

---
*Nota: casos de uso construídos com apoio de IA a partir dos requisitos funcionais e regras de negócio já mapeados. Os pontos em aberto foram mantidos explícitos em vez de assumir uma resposta não validada pelos stakeholders.*
