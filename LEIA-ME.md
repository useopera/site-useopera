# Site useopera.com.br

Página única e estática (`index.html` + `favicon.svg`). Será publicada na Vercel, no domínio useopera.com.br.

## Como ligar um produto quando ele for lançado

No fim do `index.html` existe o bloco **CONFIGURAÇÃO DOS PRODUTOS**:

```js
const PRODUTOS = {
  frota: { status: "desenvolvimento", site: "https://operafrota.com.br", planos: "https://operafrota.com.br/planos", app: "https://app.operafrota.com.br" },
  gado:  { status: "desenvolvimento", ... },
  caixa: { status: "desenvolvimento", ... },
  obra:  { status: "desenvolvimento", site: "", planos: "", app: "" }
};
```

- Trocar `"desenvolvimento"` por `"disponivel"` muda a etiqueta para **Disponível** (verde) e liga os botões **Conhecer**, **Planos** e **Entrar**.
- Botão com link vazio (`""`) continua desligado.
- Enquanto o status for `"desenvolvimento"`, a etiqueta mostra **Em desenvolvimento** e os botões ficam apagados.

## Textos
- O texto do **OperaObra** é provisório: ainda não existe especificação do produto.
- Contato: contato@useopera.com.br (ativar no Zoho antes de publicar).
