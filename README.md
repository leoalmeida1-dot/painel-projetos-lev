# Painel de Projetos Lev

Painel de gestão dos projetos sob liderança do Léo (Head de Gestão Comercial — Lev Negócios),
com rotina diária de leitura embutida.

**No ar:** https://leoalmeida1-dot.github.io/painel-projetos-lev/

## Projetos
- **CRM Lev** — substituição do Ploomes por CRM próprio
- **LEV+ (LEVAPP)** — app que integra CRM, D.Ai, PPC, Iris e Bom dia Gerente
- **D.Ai** — agente comercial de IA
- **PPC** — Programa de Progressão Comercial

> O painel do PPC é separado (`painel-ppc-lev`). Política, níveis e bônus vivem só lá.

## Visões
`Rotina do dia` · `Projetos` · `Ações` · `Kanban`

## Arquivos
- `index.html` — a aplicação (standalone, sem CDN)
- `data.json` — fonte dos dados (projetos + ações)
- `data.js` — o mesmo dado empacotado para o app (`file://` e Pages)

## Atualizar
Editar `data.json` e regerar `data.js`:

```bash
python3 -c "import json,io;d=json.load(io.open('data.json'));io.open('data.js','w').write('window.DADOS = '+json.dumps(d,ensure_ascii=False,indent=1)+';')"
```
