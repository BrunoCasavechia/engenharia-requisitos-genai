# Requisitos Não Funcionais — Sistema de Gestão de Eventos (Eventus)

O documento de elicitação afirma explicitamente que **nenhum requisito não funcional foi levantado** durante as entrevistas ("Não foram levantados requisitos relacionados à segurança, desempenho, disponibilidade, acessibilidade e privacidade dos dados.").

Por esse motivo, os itens abaixo são apresentados como **candidatos a validar** junto aos stakeholders, e não como requisitos definitivos. Foram sugeridos pela IA a partir do contexto do sistema (múltiplos usuários simultâneos, dados de pagamento, dados pessoais de participantes), mas nenhum deles deve ser considerado confirmado sem checagem com o cliente.

## Candidatos identificados

| # | Categoria | Candidato a RNF | Status |
|---|-----------|------------------|--------|
| RNF-C01 | Segurança | Dados de pagamento e dados pessoais dos participantes devem ser protegidos conforme LGPD | Candidato — a validar |
| RNF-C02 | Disponibilidade | Sistema deve estar disponível durante períodos de inscrição em eventos de alta demanda | Candidato — a validar |
| RNF-C03 | Desempenho | Controle de vagas em tempo real deve refletir mudanças sem atraso perceptível para o organizador | Candidato — a validar |
| RNF-C04 | Acessibilidade | Interface deve seguir diretrizes básicas de acessibilidade (WCAG) | Candidato — a validar |
| RNF-C05 | Privacidade | Palestrantes só devem visualizar dados de participantes estritamente necessários (ver lacuna sobre isso) | Candidato — a validar |

---
*Nota: nenhum desses itens deve ser tratado como requisito confirmado. Eles são apresentados explicitamente como lacunas de RNF, coerente com o que o próprio documento de elicitação registra.*
