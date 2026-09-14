# Logos — Grupo Komvos

Repositório **oficial e central** dos logos do Grupo Komvos.

Use este repositório como **única fonte de verdade** para logos em todos os projetos do grupo (sites, apps, painéis, materiais e integrações). Evite copiar arquivos localmente: referencie sempre os assets daqui para manter versões, nomes e identidade visual alinhados.

## Marcas

| Pasta | Marca |
| --- | --- |
| [`KOMVOS/`](./KOMVOS) | Grupo / holding Komvos |
| [`SENIOR/`](./SENIOR) | Senior |
| [`STATUM/`](./STATUM) | Statum |
| [`TRUSTH/`](./TRUSTH) | Trusth |

Cada pasta contém variações (horizontal, vertical, ícone, cores e, quando disponível, arquivo `.ai`).

## Como usar em outros projetos

### 1. URL direta (recomendado para web)

Aponte para o arquivo no `main` via raw do GitHub:

```text
https://raw.githubusercontent.com/grupo-konvos/logos-grupo-komvos/main/<MARCA>/<arquivo>.png
```

Exemplos:

```html
<img
  src="https://raw.githubusercontent.com/grupo-konvos/logos-grupo-komvos/main/KOMVOS/komvos-logo-preto.png"
  alt="Komvos"
/>
```

```css
.logo {
  background-image: url("https://raw.githubusercontent.com/grupo-konvos/logos-grupo-komvos/main/TRUSTH/logo-trusth-rosa-horizontal.png");
}
```

### 2. Git submodule

Quando o projeto precisar dos arquivos versionados localmente:

```bash
git submodule add https://github.com/grupo-konvos/logos-grupo-komvos.git assets/logos
git submodule update --init --recursive
```

Atualizar logos depois:

```bash
git submodule update --remote assets/logos
```

### 3. Clone / download pontual

```bash
git clone https://github.com/grupo-konvos/logos-grupo-komvos.git
```

Prefira URL raw ou submodule em vez de duplicar PNGs no repositório do produto.

## Convenções

- **Não altere** nomes de arquivos já publicados sem avisar os times — URLs e imports quebram.
- Novas marcas entram em pasta própria na raiz (`NOVA_MARCA/`).
- Novas variações seguem o padrão de nomenclatura da marca correspondente.
- Alterações de logo devem ser feitas **neste repositório** e propagadas aos projetos via URL ou update de submodule.

## Estrutura

```text
logos-grupo-komvos/
├── KOMVOS/
├── SENIOR/
├── STATUM/
├── TRUSTH/
└── README.md
```

---

**Fonte canônica de identidade visual do Grupo Komvos.** Todos os projetos devem consumir os logos a partir daqui.
