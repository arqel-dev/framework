# Arqel Framework — meta-package

> Atalho de instalação one-line para o stack Arqel completo.

```bash
composer require arqel-dev/framework
```

Esse comando puxa todos os pacotes core do Arqel:

- `arqel-dev/core` — service provider, registry, comandos artisan, middleware Inertia
- `arqel-dev/auth` — autorização (Policies, AbilityRegistry, panel access middleware)
- `arqel-dev/fields` — 20+ field types (text, number, date, file, relationship, etc.)
- `arqel-dev/form` — form builder com validation + FormRequest auto-generation
- `arqel-dev/actions` — Actions com side-effects, autorização, confirmation
- `arqel-dev/nav` — sidebar/topbar nav primitives
- `arqel-dev/table` — table builder (columns, filters, sorting, pagination)
- `inertiajs/inertia-laravel` — bridge PHP↔React (estado default da framework)

Para pacotes opcionais (`audit`, `tenant`, `workflow`, `versioning`, `marketplace`, `mcp`, `ai`, `realtime`, `widgets`, `fields-advanced`, `cli`, `export`), instala-os caso a caso:

```bash
composer require arqel-dev/audit
composer require arqel-dev/tenant
# etc.
```

## Documentação

- Site: <https://arqel.dev>
- Source code: <https://github.com/arqel-dev/arqel>
- Issues: <https://github.com/arqel-dev/arqel/issues>

## Sobre este repositório

Este repo contém apenas o `composer.json` que declara o meta-package. Não tem código PHP — `type: metapackage` significa que o Composer só trata as dependências declaradas em `require` sem instalar nada do próprio repo.

A versão deste meta-package é mantida em sincronia com a release da framework no monorepo principal ([`arqel-dev/arqel`](https://github.com/arqel-dev/arqel)). Cada release tem uma tag aqui também.

## Licença

MIT — ver [`LICENSE`](https://github.com/arqel-dev/arqel/blob/main/LICENSE) no monorepo.
