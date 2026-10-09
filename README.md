# BIREME OPS Customizations

Customizações e correções aplicadas ao Open Preprint Systems (OPS)
utilizado pelo BIREME Preprints.

## Ambiente de referência

- OPS: 3.5.0-4
- Organização: BIREME/OPAS/OMS

## Patches

### fix-competing-interests-ptbr.patch

Corrige o rótulo do campo de conflito de interesses no formulário
de submissão.

Arquivo original:
locale/pt_BR/author.po

Problema:
A tradução original contém HTML e uma variável Smarty que são
exibidos literalmente no formulário.

Correção:
Substitui a tradução por "Conflito de interesses".

## Aplicação

A partir da raiz do OPS, verificar primeiro:

git apply --check /caminho/para/fix-competing-interests-ptbr.patch

Se a verificação for bem-sucedida:

git apply /caminho/para/fix-competing-interests-ptbr.patch

ATENÇÃO:
Não aplicar em uma instalação que já contenha a correção.

Antes de atualizar o OPS, verificar se o patch continua necessário.
