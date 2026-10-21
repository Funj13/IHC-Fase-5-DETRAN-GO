# Checklist de credenciais e cenários — V1.0

## Dados fictícios

| Cenário | Placa | Renavam | Resultado esperado |
|---|---|---|---|
| A — Com débitos | ABC1D23 | 12345678901 | IPVA e licenciamento selecionáveis |
| B — Sem débitos | XYZ9Z99 | 10987654321 | Nenhum débito encontrado |
| C — Erro | ABC1D23 | 12345 | Orientação para corrigir dados e possibilidade de retorno |

O protótipo reconhece esses cenários fechados. Não valida identificadores oficiais e não consulta qualquer cadastro real. Nenhum login Gov.br, banco ou credencial pessoal é necessário. A conta do Proto.io é necessária para editar; o acesso pelo link de participante deve ser conferido antes da sessão.

Valores: IPVA R$ 850,00; licenciamento R$ 168,60; ambos R$ 1.018,60. Vencimentos fictícios: 15/09/2026 e 30/11/2026. A classificação “Vencido”/“A vencer” usa a data de referência fixa de 20/10/2026, não o relógio real.

## Acesso e sessão

- [ ] Link de participante abre sem permissão de edição e foi conferido em janela anônima.
- [ ] Eventual senha de visualização está documentada para o professor e o moderador.
- [ ] Disponibilidade do link e validade do plano Proto.io conferidas antes dos testes.
- [ ] Versão V1.0 identificada; mudanças posteriores não são misturadas com os resultados dessa versão.
- [ ] Navegador, dispositivo e escala padronizados.
- [ ] Player recarregado antes de cada participante.
- [ ] Cronômetro e ficha de métricas prontos.

## Cenários funcionais

- [ ] Home leva ao formulário e o retorno funciona.
- [ ] Os dois campos aceitam edição e apresentam instruções em português.
- [ ] Ajuda do Renavam abre, fecha e preserva dados de consulta.
- [ ] Consulta vazia e Renavam incompleto não levam ao extrato.
- [ ] Cenário A mostra os dois débitos; cenário B mostra ausência de débitos.
- [ ] Seleção inicial vazia; continuação sem seleção é bloqueada.
- [ ] Seleção e remoção de IPVA atualizam o total.
- [ ] Seleção e remoção de licenciamento atualizam o total.
- [ ] Ambos selecionados somam R$ 1.018,60.
- [ ] Revisão preserva somente os itens escolhidos e o total correspondente.
- [ ] Voltar para editar preserva a seleção.
- [ ] Gerar/clicar em copiar Pix mantém o pagamento pendente.
- [ ] Cópia está identificada como simulação; não pressupor alteração real da área de transferência.
- [ ] Expiração permite nova geração sem alterar o valor.
- [ ] Confirmação ocorre apenas após evento do moderador e mostra resumo coerente.
- [ ] Controles do moderador não são executados pelo participante.

Marcar os itens somente após a verificação correspondente; este checklist não é um relatório de resultados com usuários.
