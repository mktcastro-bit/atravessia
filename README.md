# A TRAVESSIA — Do véu à consciência

Roteiro para uma vivência – uma travessia – com sound healing.
Uma jornada sonora, corporal, vocal e simbólica de despertar.

**Duração:** 1h20 · **Estrutura:** 6 etapas/movimentos

> Projeto autoral em desenvolvimento. Este repositório é o caderno de trabalho da criação.

---

## Conteúdo

| Arquivo | O que é |
|---|---|
| `roteiro.md` | O roteiro, íntegra. Fonte da verdade do projeto. |
| `index.html` | **Partitura visual** — o mesmo roteiro reorganizado na horizontal, em quatro camadas. Abrir direto no navegador. |
| `CHANGELOG.md` | Registro das versões. |

### Sobre a partitura visual

A partitura reorganiza o roteiro: os movimentos lado a lado na horizontal, com as
transições entre eles, e o conteúdo de cada um distribuído em quatro camadas —
paisagem sonora, corpo e movimento, voz e condução, estado/elemento/centro. Acima,
uma faixa de participação e uma linha de tempo.

O que a partitura propôs a pedido do autor — o nome de um movimento, um elemento,
um estado — está marcado como *proposta*, no roteiro e na partitura; a nota ao fim
da página foi redigida a pedido dele. Onde o roteiro ainda não especifica uma
camada, a célula diz *não especificado*, em vez de preenchida por suposição.

Clicar num movimento ou numa transição abre o trecho integral. Os botões no topo
isolam uma camada por vez.

### Acesso

A página abre com um portal de entrada. Credenciais atuais: **login `vida` · senha `vida`**.
Para trocar, edite a constante `ACESSO` no início do `<script>` em `index.html`.

> ⚠️ **Barreira simbólica, não segurança real.** As credenciais ficam no código-fonte da
> página e são legíveis por qualquer pessoa com conhecimento técnico. Serve para manter a
> página fora do alcance casual de quem receber o link. A proteção efetiva vem de o
> repositório ser privado.

---

## Como editar

O texto do roteiro vive em dois lugares e precisa ser mantido em sincronia:

1. `roteiro.md` — a íntegra.
2. `index.html` — na constante `PHASES`, no topo do `<script>`. Um objeto por movimento,
   com as chaves `som`, `corpo`, `voz`, `simb` (as quatro camadas) e `texto` (o trecho
   integral que aparece no painel de detalhe). Não é preciso mexer em HTML nem em CSS.

Camada sem conteúdo = array vazio `[]`. A célula se marca sozinha como não especificada.

---

© Luciano Castro. Todos os direitos reservados.
Obra autoral em desenvolvimento — reprodução, adaptação ou condução por terceiros
não autorizadas.
