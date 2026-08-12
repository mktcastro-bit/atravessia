# A TRAVESSIA — Do véu à consciência

Vivência sonora, corporal, vocal e simbólica de despertar.
Experiência de som, corpo, respiração, movimento, voz, imaginação e símbolo.

**Duração:** 2h15 – 2h30 · **Estrutura:** 6 movimentos

> Projeto autoral em desenvolvimento. Este repositório é o caderno de trabalho da criação:
> roteiro, dramaturgia, camadas sonoras e registro das versões ao longo dos testes.

---

## Conteúdo

| Arquivo | O que é |
|---|---|
| `index.html` | **Partitura visual** — linha do tempo interativa das 2h30, com curva de intensidade energética e 4 camadas (paisagem sonora, corpo, voz, símbolo). Abrir direto no navegador. |
| `roteiro.md` | Roteiro completo em texto, movimento a movimento. |
| `CHANGELOG.md` | Registro das versões e do que mudou a cada teste com grupo. |

### Acesso à partitura

A página abre com um portal de entrada. Credenciais atuais: **login `vida` · senha `vida`**.
Para trocar, edite a constante `ACESSO` no início do `<script>` em `index.html`.

> ⚠️ **Isto é uma barreira simbólica, não segurança real.** As credenciais ficam no
> código-fonte da página e qualquer pessoa com conhecimento técnico consegue lê-las
> em segundos. Serve para manter a página fora do alcance casual de quem receber o
> link — não para proteger a obra de quem quiser mesmo acessá-la. A proteção efetiva
> vem de o repositório ser privado.

---

## Arco dramatúrgico

```
tomar consciência do corpo
  → despertar o instinto
    → reunir a força
      → atravessar o fogo
        → aquietar
          → ascender
            → encontrar a sabedoria
              → celebrar e retornar
```

## Os seis movimentos

| # | Movimento | Min | Elemento | Estado |
|---|---|---|---|---|
| I | Abertura | 30 | espaço / água | repouso, receptividade |
| II | A Floresta | 20 | terra | instinto, espontaneidade |
| III | O Batalhão | 25 | terra / fogo | força, poder coletivo |
| IV | O Fogo | 20 | fogo | transmutação |
| V | A Ascensão *(nome provisório)* | 30 | éter | integração, desaceleração |
| VI | O Despertar | 25 | luz | alegria, comunhão |

Arquétipos ativados: O Louco · O Guerreiro · O Mago · O Sol · O Sábio · O Mundo.

---

## Como editar a partitura visual

Todo o conteúdo da linha do tempo vive em **um único bloco de dados** no topo do
`<script>` em `index.html` — a constante `PHASES`. Não é preciso mexer em HTML ou CSS.

Cada movimento tem esta forma:

```js
{
  id:"IV", nome:"O FOGO", tag:"Poder e transformação · o Mago",
  min:20,                 // duração em minutos → define a largura na linha do tempo
  cor:"var(--c4)",
  e:[.85, 1, .62],        // intensidade energética (0 a 1) no início / meio / fim
  estado:"...", elemento:"fogo", centro:"plexo solar", arquetipo:"O Mago",
  som:[   ...ítens da camada Paisagem sonora & instrumentos ],
  corpo:[ ...ítens da camada Corpo & movimento ],
  voz:[   ...ítens da camada Voz & condução ],
  simb:[  ...ítens da camada Símbolo & arquétipo ],
  texto:`<p>descrição longa que aparece no painel de detalhe</p>`
}
```

Ajustes comuns:

- **mudar a duração de uma etapa** → altere `min`. As larguras se recalculam sozinhas.
- **mudar a curva de energia** → altere os três valores de `e`.
- **frase de condução em destaque** → dentro de `voz`, envolva em `<q>...</q>`.
- **acrescentar uma camada nova** (ex.: iluminação, aromas) → adicione a chave em cada
  movimento e registre-a no array `LAYERS`.

---

## Aberto / a definir

- [ ] Nome definitivo do movimento V (candidatos: A Ascensão · O Pouso · A Rendição · O Ar · A Clareira)
- [ ] Instrumentação definitiva por etapa
- [ ] Repertório de cantos e vocalizações autorais
- [ ] Testes com grupo-piloto
- [ ] Ajuste fino dos tempos a partir dos testes

---

© Luciano Castro. Todos os direitos reservados.
Obra autoral em desenvolvimento — reprodução, adaptação ou condução por terceiros
não autorizadas.
