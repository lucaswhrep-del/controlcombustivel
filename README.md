# Controle de Combustivel

App web para registro diario de quilometragem, conferencia por fotos, aprovacao mensal e pagamento de combustivel para supervisores.

## Publicacao no Netlify

- Build command: deixe vazio
- Publish directory: `.`
- Arquivo principal: `index.html`

## Firebase

O app usa Firebase como servidor. Antes de usar em producao, confirme no Firebase Console:

- Authentication com `Anonymous` habilitado
- Firestore Database criado
- Storage criado
- Regras publicadas a partir de `firestore.rules` e `storage.rules`

## Usuarios iniciais

```text
admin / admin123
financeiro / fin123
supervisor / sup123
```

