# Mapa de telas e interações nativas

| Tela | Finalidade |
|---|---|
| 01 · Início | Localizar o serviço de consulta de débitos |
| 02 · Consultar veículo | Informar placa e Renavam e validar os cenários de teste |
| 03 · Ajuda Renavam | Orientar a localização do código no CRLV fictício |
| 04 · Débitos do veículo | Selecionar IPVA/licenciamento e conferir total |
| 05 · Revisar seleção | Conferir itens e valor, editar seleção ou gerar Pix |
| 06 · Pix aguardando | Exibir código ilustrativo, cópia simulada e estado pendente |
| 07 · Pix expirado | Recuperar o fluxo gerando outro código simulado |
| 08 · Pagamento confirmado | Exibir confirmação e resumo sem transação real |
| 09 · Corrigir dados | Recuperação da consulta com dados inválidos |
| 10 · Selecione um débito | Recuperação de tentativa de continuar sem seleção |
| 11 · Sem débitos | Resultado do cenário fictício sem pendências |

## Modelo de interação

O protótipo utiliza textos, botões, campos e checkboxes nativos do Proto.io. As ações usam navegação entre telas, variáveis, expressões e alteração de propriedades. Não utiliza site auxiliar, Web View ou componente HTML.

Consulta → validação → extrato → seleção → revisão → Pix pendente → confirmação acionada pelo moderador.

Ramificações: ajuda do Renavam; dados inválidos; consulta sem débitos; seleção vazia; Pix expirado e nova geração.

## Limites da simulação

- Não há integração com DETRAN, Gov.br ou banco.
- Somente os dados documentados no checklist representam cenários disponíveis.
- O código e o símbolo do QR Code não são instruções válidas de pagamento.
- A cópia é um feedback simulado; não é uma integração com a área de transferência.
- O moderador dispara expiração e confirmação em controles próprios.
- A seleção individual é uma hipótese de interação do projeto; regras de quitação do serviço real precisariam ser validadas.
- A adaptação para outros tamanhos de tela e conformidade integral de acessibilidade exigiriam avaliação adicional.
