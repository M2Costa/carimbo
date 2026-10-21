# Carimbo

Kit de marca para médicos em início de carreira, já em conformidade com a Resolução CFM 2.336/2023. Projeto autoral de Matheus Morato da Costa.

> Sua marca já nasce com CRM.

## Estrutura

| Pasta | Conteúdo |
|---|---|
| `site/` | Landing page do MVP (`index.html`, um arquivo só, sem build) |
| `brand/logo/` | Símbolo e logotipo em SVG; `png/` traz o símbolo em 1024, 512 e 256 px |
| `design/canvas/` | Pranchas da identidade visual (nome, logo, símbolo, cores, tipografia, aplicações) |
| `design/apresentacao/` | Slides da apresentação da marca |

## Landing page

Abra `site/index.html` no navegador. A página tem cabeçalho, apresentação do produto, benefícios, lista de espera, perguntas frequentes e rodapé.

### Lista de espera

- **No claude.ai** (versão publicada como Artifact), as inscrições ficam no banco de dados da página, uma por pessoa, visíveis só para o dono.
- **Fora do claude.ai**, o formulário envia um `POST` com o JSON da inscrição para `FORM_ENDPOINT`, no início do `<script>` em `site/index.html`. Preencha com o endereço de um serviço de formulários (por exemplo, um endpoint do Formspree). Vazio, o formulário avisa que não conseguiu salvar.

Campos enviados: `nome`, `email`, `especialidade`, `uf`, `momento`, `interesses`, `preco`, `consentimento`, `origem`, `atualizadoEm`.

### Antes de divulgar

Preencha os contatos do rodapé: `[e-mail de contato]`, `[WhatsApp]`, `[@perfil]` e `[página]`.

## Identidade

| Cor | Hex | Uso |
|---|---|---|
| Verde Prontuário | `#12302F` | Textos, logotipo, fundos de destaque |
| Verde Clínico | `#1F6F66` | Subtítulos, links, ícones |
| Tinta | `#E2582B` | Acento: módulo livre do símbolo, botões |
| Tinta escura | `#B9441C` | Texto pequeno em laranja sobre fundo claro |
| Menta | `#DCEBE6` | Fundos de apoio |
| Névoa | `#EEF3F1` | Fundo principal |

Tipografia: **Source Serif 4** (títulos e logotipo) e **Source Sans 3** (texto), ambas do Google Fonts.

Os SVGs do logotipo completo usam o texto "carimbo" em Source Serif 4 Bold, sem conversão em curvas; instale a fonte para abrir em editores como Illustrator. Os SVGs do símbolo são só formas.
