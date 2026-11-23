# LevelUp — versão individual, sem cadastro

Aplicativo Android feito com Expo e React Native. Abre diretamente na tela inicial, sem autenticação, Supabase ou cadastro.

## Recursos

- Missões com título, descrição, categoria e recompensa em XP.
- Criar, editar, concluir e excluir missões.
- Níveis, barra de progresso e ofensiva diária.
- Perfil personalizável com avatar, nome, bio e cor de destaque.
- Conquistas desbloqueadas pelo progresso.
- Desafios pessoais com duração e conclusão.
- Salvamento local no aparelho com AsyncStorage.

## Requisitos

- Node.js 22 ou superior.
- Conta Expo para gerar APK com EAS Build.

## Executar localmente

```bash
npm install
npx expo start --clear
```

## Gerar APK no Android

```bash
npm install -g eas-cli
eas login
eas build:configure
eas build -p android --profile preview
```

No PowerShell, se o EAS não encontrar Git:

```powershell
$env:EAS_NO_VCS="1"
eas build -p android --profile preview
```

O EAS compila na nuvem e fornece um link para baixar o APK.

## Dados

O progresso fica salvo no próprio celular. Cada aparelho tem seu próprio perfil e progresso; amigos e sincronização online não fazem parte desta versão.
