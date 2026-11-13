# Catálogo de APIs Públicas

Lista em JSON de APIs que podem ser usadas em aulas, exercícios e protótipos. O catálogo reúne opções de jogos, filmes, ciência, clima, receitas, animais e outros temas.

## Arquivo

- `api-publica.json`: objeto com a propriedade `apis`.

Cada entrada possui:

```json
{
  "name": "Nome da API",
  "theme": "Categoria",
  "base_url": "URL base",
  "description": "Resumo do serviço"
}
```

## Como consumir

```js
const response = await fetch(
  "https://raw.githubusercontent.com/ProfLucasSousa/apis-publicas/main/api-publica.json"
);
const { apis } = await response.json();

console.table(apis);
```

## Atenção

Este arquivo é um catálogo, não um proxy. Cada serviço possui regras próprias de autenticação, limites de requisição e disponibilidade. Consulte a documentação oficial da API escolhida antes de usá-la em um projeto.
