# Configuracao Firebase

Este app ja esta preparado para usar Firebase como servidor.

## 1. Criar projeto

1. Acesse https://console.firebase.google.com
2. Crie um projeto.
3. Adicione um app Web.
4. Copie o objeto `firebaseConfig`.

## 2. Configuracao no app

O `firebaseConfig` do projeto `control-combustivel` ja foi inserido no arquivo `controle-combustivel-supervisores.html`.

## 3. Ativar produtos

No Firebase Console, ative:

- Authentication: habilite `Anonymous`.
- Firestore Database: crie em modo producao.
- Storage: crie o bucket padrao.

## 4. Publicar regras

Use os arquivos:

- `firestore.rules`
- `storage.rules`

Observacao: estas regras servem para o MVP funcionar com login anonimo do app. Para producao real, o ideal e evoluir para Firebase Auth com usuarios reais e regras por perfil.

## 5. Netlify

Pode publicar este HTML no Netlify. Todos os computadores/celulares usando a mesma URL passam a ler e gravar no mesmo Firestore/Storage.

O app esta configurado para funcionar somente com Firebase. Se Auth, Firestore ou Storage nao estiverem disponiveis, o login fica bloqueado para evitar registros salvos apenas no navegador.
