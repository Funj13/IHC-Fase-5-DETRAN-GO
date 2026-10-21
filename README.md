# IHC-Fase-5-DETRAN-GO

Protótipo acadêmico da Fase 5 de IHC: consulta de débitos de veículo e pagamento Pix simulado, seguindo o fluxo avaliado na Fase 4.

## Protótipo no Proto.io

- [Abrir player do protótipo](https://caiquepires.proto.io/player/index.cfm?id=22109947-a29d-4887-b7e6-1bfb1deb4f2d)
- [Abrir projeto no editor (requer acesso à conta)](https://caiquepires.proto.io/editor/index.cfm?id=22109947-a29d-4887-b7e6-1bfb1deb4f2d)

O projeto usa componentes nativos do Proto.io. Há 11 telas: início, consulta, ajuda Renavam, débitos, revisão, Pix aguardando, Pix expirado, confirmação, erro de dados, seleção vazia e ausência de débitos.


## Documentos

- [Roteiro com seis tarefas e métricas](fase-5/roteiro-de-teste.md)
- [Checklist de credenciais e cenários](fase-5/checklist-de-cenarios.md)
- [Planilha para registrar métricas](fase-5/registro-de-metricas.csv)
- [Matriz de telas e interações previstas](fase-5/matriz-de-interacoes.md)
- [Melhorias e delimitação do escopo](fase-5/melhorias-da-fase-4.md)

## Dados fictícios

| Cenário | Placa | Renavam | Resultado previsto |
|---|---|---|---|
| Com débitos | ABC1D23 | 12345678901 | IPVA R$ 850,00 e licenciamento R$ 168,60 |
| Sem débitos | XYZ9Z99 | 10987654321 | Mensagem de ausência de débitos |
| Erro | ABC1D23 | 12345 | Orientação para corrigir os dados |

Nenhum pagamento é realizado. QR, código Pix, cópia e confirmação são simulações para avaliação de usabilidade. Usar somente os dados fictícios acima. Os documentos descrevem o comportamento planejado; os itens do checklist só devem ser marcados após verificação no player.
