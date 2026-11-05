# Bestiário de Arton — Raças

Módulo para **Foundry VTT** que adiciona ao sistema **Tormenta20** as raças jogáveis
apresentadas no **Apêndice A — Raças para Personagens** do *Bestiário de Arton*.

> **Id do módulo:** `bestiario-de-arton-racas`
> **Autor:** @xx_.luis._xx
> **Versão:** 1.1.0

---

## Instalação rápida no Foundry

Em **Add-on Modules → Install Module**, cole isto no campo **URL do Manifesto**:

```
https://github.com/Luisguilhermelr/bestiario-de-arton-racas/releases/latest/download/module.json
```

Clique em **Install** e depois ative o módulo em **Gerenciar Módulos**.
O Foundry baixa e atualiza o módulo sozinho a partir dessa URL.

> Repositório: https://github.com/Luisguilhermelr/bestiario-de-arton-racas

---

## Conteúdo

O compêndio de Itens **Raças do Bestiário de Arton** (`packs/racas`) contém três pastas,
com **45 itens** no total — **5 raças e 40 poderes** — conferidos no compêndio:

- **Raças** — as 5 raças da Tabela A-1:
  - Elfo-do-Gelo
  - Lâmia
  - Manotauro
  - Salamandra
  - Vampiro
- **Poderes Raciais** — os poderes de cada raça, já vinculados aos `grants` das raças
  correspondentes, além dos poderes opcionais que não entram automaticamente na ficha.
- **Licantropia (Lobisomem)** — as habilidades de licantropia, usadas como itens de
  habilidade (`type: poder`) e não como uma raça.

### Poderes automáticos por raça

| Raça | Poderes concedidos |
| --- | --- |
| Elfo-do-Gelo | Graça de Beluhga, Herança Gélida, Sentidos Glaciais |
| Lâmia | Corpo Felino, Magia das Lâmias, Natureza Predadora, Toque Psíquico |
| Manotauro | Cascos, Chifres, Corpulento, Medo de Altura |
| Salamandra | Calor Natural, Cauda, Cria das Chamas, Fraqueza Glacial |
| Vampiro | Bênçãos Vampíricas, Resquícios da Outra Vida, Natureza Não Viva, Perda da Humanidade |

### Poderes opcionais

- **Alma da Fornalha** (Salamandra) — poder de raça de 7º nível, deve ser adicionado
  manualmente à ficha no lugar de um poder de classe.
- **Bênçãos Vampíricas individuais** — as 11 bênçãos descritas no poder agregado
  *Bênçãos Vampíricas* também estão no compêndio como itens separados, para serem
  adicionadas à ficha quando o jogador escolher cada uma:
  Cura Acelerada, Dominação Vampírica, Drenar Sangue, Forma de Lobo, Forma de Morcego,
  Garras, Manto das Sombras, Passo Vampírico, Predador Sorrateiro, Presença Majestosa
  e Resiliência Sombria.

### Licantropia (Lobisomem)

As habilidades de lobisomem estão na pasta **Licantropia (Lobisomem)** e são itens de
habilidade (`type: poder`), não uma raça. São elas:

- **Habilidades de Lobisomem** — item-resumo com todas as habilidades e as formas.
- **Aversão a Mitral** — fraqueza: dano extra e perda de vida com mitral.
- **Empatia com Lobos** — bônus com lobos e lobos-das-cavernas.
- **Maldição da Licantropia** — a mordida transmite licantropia (Fort CD Con).
- **Sentidos Aguçados** — concede faro e visão na penumbra (com efeito automático).
- **Transformação Incontrolável** — efeitos da licantropia e perda de controle.
- **Forma Híbrida** — forma de combate, com ataques naturais e efeito de +2 em Força.
- **Forma de Lobo** — forma de lobo, com deslocamento 15m e efeito de +2 em Força.
- **Controlar Licantropia** — poder de destino (geral) para controlar a transformação.

> **Uso das formas:** os efeitos de *Forma Híbrida* e *Forma de Lobo* vêm **desativados
> por padrão**. Ative o efeito do item ao assumir a forma e desative ao voltar à forma
> humanoide.

## Automação

Os poderes trazem **Active Effects** embutidos (16 efeitos no compêndio) para os bônus
mais diretos: deslocamento, tamanho, sentidos, redução de dano/imunidade, perícias e
imunidades a condições.
Efeitos que dependem de escolhas, cenas ou uso ativo de PM ficam apenas descritos no
texto do poder.

## Instalação manual

1. Feche o Foundry (ou apenas recarregue com `F5` depois).
2. Copie a pasta `bestiario-de-arton-racas` para:
   - Windows: `%LOCALAPPDATA%\FoundryVTT\Data\modules\`
   - Linux: `~/.local/share/FoundryVTT/Data/modules/`
3. Abra o Foundry e entre no mundo com o sistema **Tormenta20**.
4. Em **Gerenciar Módulos**, ative **Bestiário de Arton — Raças**.
5. Recarregue a página com `F5`.
6. Abra o compêndio **Raças do Bestiário de Arton** e arraste a raça desejada para a ficha.

> Se a opção *Abrir raças* estiver ativa no sistema, arrastar a raça abre o diálogo de
> distribuição dos atributos dinâmicos. Isso é o comportamento esperado.

## Requisitos

- Foundry VTT **13 ou 14**
- Sistema **Tormenta20 1.5+** (verificado em 1.6.5)

## Observações

- Conteúdo extraído do Apêndice A do *Bestiário de Arton* (Jambô). Não comercializar
  este módulo nem seu conteúdo.
- Compatível com Foundry VTT 13/14 e Tormenta20 1.5+.

---

Feito por **@xx_.luis._xx**.
