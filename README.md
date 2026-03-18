# Arxiv Package

Pacote consolidado para a vitrine no arXiv:

- `main.tex` é a única fonte LaTeX do manuscrito.
- `artigos_icpr.bib` concentra as referências usadas na revisão.
- O estilo Elsevier/CIE foi mantido apenas como baseline editorial.

## Estrutura

- `main.tex`
- `artigos_icpr.bib`
- `highlights.txt`
- `data_extraction.xls`
- `supplementary/README.md`
- `supplementary/docs/review_audit_trail.md`
- `supplementary/docs/included_studies.md`
- `supplementary/docs/full_text_availability_note.md`
- `figures/prisma_flow_diagram.pdf`
- `figures/corpus_evidence_maps.pdf`

## Compilação

```bash
latexmk -pdf main.tex
```

## O que revisar antes de publicar no arXiv

- Confirmar se a autoria pública em `main.tex` já representa a equipe final.
- Revisar a seção de disponibilidade de dados conforme a estratégia final de compartilhamento e o nível de abertura desejado para os materiais suplementares.
- Atualizar `highlights.txt` apenas se o pacote for reaproveitado para submissão futura.

## Checklist editorial rápida

- [x] `main.tex` é a única fonte LaTeX do pacote.
- [x] `artigos_icpr.bib` está ligado ao build do manuscrito.
- [x] `abstract` está abaixo do limite do CIE: 207 / 250 palavras.
- [x] `keywords` estão dentro da faixa pedida pelo CIE: 5 / 7.
- [x] `highlights.txt` atende a regra de 3 a 5 bullets com até 85 caracteres por bullet.
- [x] O corpo do artigo está organizado em seções numeradas.
- [x] O pacote agora inclui um trilho metodológico mínimo com apêndices e notas suplementares.
- [x] O pacote registra que o guia atual não explicita um teto fixo de páginas ou palavras para o corpo.

## Pendências de decisão da equipe

- [ ] Confirmar se a autoria pública atual é a lista final da vitrine.
- [ ] Revisar se as `keywords` devem ser encurtadas para ficar mais próximas da recomendação do guia.
- [ ] Decidir se o pacote será divulgado como transparência parcial ou apenas após recuperar o workspace completo do Parsifal.
- [ ] Decidir se vale produzir `graphical abstract` para um uso futuro em submissão.

## Padrão editorial adotado

- `Highlights` são obrigatórios em um eventual fluxo de submissão.
- `Graphical abstract` é opcional.
- O guia atual não explicita um limite fixo de páginas ou palavras para o corpo.
- O texto deve usar seções numeradas com clareza e referências em estilo `APA`.
- O guia informa que compartilhar `preprints`, como em um servidor de preprints, não conta como publicação prévia.

Fontes oficiais consultadas em 2026-03-15:

- https://www.sciencedirect.com/journal/computers-and-industrial-engineering/publish/guide-for-authors
- https://www.sciencedirect.com/journal/computers-and-industrial-engineering/about/aims-and-scope
- https://www.elsevier.com/about/policies-and-standards/sharing
