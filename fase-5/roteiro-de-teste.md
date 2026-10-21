# Roteiro de teste de usabilidade — V1.0

Grupo: Quarteto da TI. Interface: protótipo acadêmico do DETRAN-GO, construído com componentes nativos do Proto.io.

## Objetivo e escopo

Avaliar a localização do serviço, a compreensão dos campos, a recuperação de erros, a seleção individual de débitos e a distinção entre Pix pendente e confirmação simulada. O fluxo dá continuidade à fase 4, que delimitou consulta e pagamento de débitos veiculares. As fases iniciais abordavam CNH; essa mudança de escopo deve ser registrada no relatório geral. Os cenários das personas devem ser adaptados e identificados como hipóteses de projeto.

## Preparação

- Teste moderado individual; duração estimada de 20–30 minutos.
- Realizar um piloto antes da rodada com participantes. Na fase 6, a proposta prevê 2–5 testes.
- Usar a mesma versão, navegador, escala e dispositivo em cada sessão comparável.
- Identificar participantes como P01, P02 etc.; não coletar CPF, placa ou dados bancários reais.
- Recarregar o player entre participantes. A navegação para o início não equivale necessariamente a limpar a sessão.
- Usar cronômetro e a ficha `registro-de-metricas.csv`. Resultados permanecem vazios até a execução com usuários.

## Abertura

“Estamos avaliando a interface. Use apenas os dados fictícios fornecidos e diga em voz alta o que procura e o que espera que aconteça. Nenhum pagamento real será feito. Você pode interromper a atividade a qualquer momento.”

Solicitar autorização específica se houver gravação. Não gravar sem autorização.

## Tarefas

Não mostrar a coluna de preparação ou os critérios de sucesso ao participante.

| ID | Enunciado ao participante | Preparação do moderador | Sucesso independente |
|---|---|---|---|
| T1 | Você quer verificar se há valores pendentes para seu veículo. Encontre onde fazer essa consulta. | Iniciar na Home. | Abrir o formulário de consulta. |
| T2 | Você tem o documento do veículo, mas não sabe onde localizar o Renavam. Descubra essa informação e retorne à consulta. | Formulário aberto. | Encontrar a ajuda, explicar onde procuraria o código e retornar. |
| T3 | Consulte o veículo com os dados fornecidos. O Renavam anotado inicialmente está incompleto; corrija-o quando perceber o problema. | Fornecer placa ABC1D23 e Renavam inicial 12345; informar o número completo 12345678901 após a tentativa, sem orientar a navegação. | Identificar o impedimento, retornar, corrigir o número e abrir o extrato. Registrar a entrega do dado como parte planejada do cenário, não como ajuda de navegação. |
| T4 | Você quer pagar somente o licenciamento. Prepare o pagamento e confira o valor antes de continuar. | Extrato com seleção zerada. | Revisão mostra somente licenciamento e R$ 168,60. |
| T5 | Prepare o pagamento por Pix usando a opção de copiar o código. Depois diga se o pagamento já foi concluído. | Revisão com licenciamento selecionado. | Acessar Pix, acionar a cópia simulada e reconhecer o estado aguardando pagamento. A área de transferência real não é avaliada. |
| T6 | O código expirou antes de você terminar. Consiga um novo código e, após a confirmação do ambiente de teste, localize o resultado. | Moderador aciona “expirar”; após a nova geração, aciona “confirmar”. | Gerar outro código, manter o valor e reconhecer a confirmação simulada. |

Os controles “Moderador” são usados somente pelo condutor do teste. Não orientar o participante a acioná-los. Entre tarefas, preparar o próximo estado se a tarefa anterior falhar e registrar a intervenção; uma falha não deve inviabilizar a sequência.

## Métricas e regras

- **Independente:** concluiu sem indicação do caminho.
- **Com ajuda:** concluiu após orientação do caminho; descrever a orientação.
- **Não concluiu:** desistiu, atingiu o limite ou não chegou ao resultado.
- **Falha técnica:** problema do protótipo; registrar separadamente e repetir após restaurar o estado, quando viável.
- **Tempo:** do fim da leitura do enunciado até o critério de conclusão ou encerramento. Registrar segundos.
- **Erros:** tentativas de consulta inválidas, escolhas incorretas e ações que afastam do objetivo; contar e descrever.
- **Comentários:** registrar falas literais relevantes, hesitações e interpretação do status.

Limite operacional sugerido: três minutos por tarefa, ajustável após o piloto e fixado antes da rodada. Perguntas neutras permitidas: “O que você espera que aconteça?” e “O que está procurando?”.

Taxa de sucesso independente por tarefa = conclusões independentes / tentativas válidas × 100. Informar também contagens brutas, sucessos com ajuda, falhas técnicas e mediana dos tempos. Não misturar falha técnica com falha de usabilidade.

## Encerramento

Perguntar: “O que foi mais difícil?”, “Em algum momento você achou que o pagamento já tinha acontecido?” e “O que mudaria primeiro?”. Os resultados e as correções resultantes serão documentados na fase 6.
