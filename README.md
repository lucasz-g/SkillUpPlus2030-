# SkillUpPlus 2030+

## Integrantes
Lucas Garcia - RM554070


Iago Diniz - RM553776


Pedro Henrique - RM553988 

## Descrição do Projeto

O **SkillUpPlus 2030+** é um aplicativo móvel desenvolvido em **React Native** (utilizando **Expo Router**) para apoiar trabalhadores e estudantes na requalificação profissional frente às transformações do mercado, inspirando-se nos ODS 4 (Educação de Qualidade) e ODS 8 (Trabalho Decente e Crescimento Econômico).

O aplicativo implementa uma **estrutura de navegação híbrida** (Stack, Drawer e Tab Navigation) e utiliza componentes nativos do React Native, Hooks e persistência de dados (AsyncStorage) para simular o login e salvar informações do usuário.

## Estrutura de Navegação

1.  **Stack Navigation (Fluxo Sequencial):**
    *   `index.tsx` (Tela de Login/Boas-vindas) -> `(drawer)` (Tela Principal)

2.  **Drawer Navigation (Menu Lateral):**
    *   Agrupa as principais seções do aplicativo:
        *   `(tabs)`: Grupo de navegação principal (Home, Autoavaliação, Trilhas, Progresso).
        *   `profile`: Tela de Perfil.
        *   `settings`: Tela de Configurações.

3.  **Tab Navigation (Abas Inferiores):**
    *   Agrupa as funcionalidades centrais do aplicativo:
        *   `home`: Tela Inicial.
        *   `assessment`: Tela de Autoavaliação (com formulário e Picker).
        *   `trilhas`: Tela de Trilhas de Aprendizado (com ScrollView).
        *   `progress`: Tela de Monitoramento de Progresso.

## Tecnologias Utilizadas

*   **Framework:** React Native (com Expo)
*   **Roteamento:** Expo Router
*   **Navegação:** `@react-navigation/drawer`, `@react-navigation/bottom-tabs`, `@react-navigation/stack`
*   **Persistência de Dados:** `@react-native-async-storage/async-storage`
*   **Componentes:** `View`, `ScrollView`, `TextInput`, `Text`, `Button`, `Image`, `StyleSheet`, `TouchableOpacity`, `Alert`, `Picker`.

## Estrutura de Diretórios

```
SkillUpPlus2030Plus/
├── app/
│   ├── (drawer)/
│   │   ├── (tabs)/
│   │   │   ├── _layout.tsx         # Layout da Tab Navigation
│   │   │   ├── home.tsx            # Tela Home
│   │   │   ├── assessment.tsx      # Tela de Autoavaliação (Formulário/Picker)
│   │   │   ├── trilhas.tsx         # Tela de Trilhas (ScrollView)
│   │   │   └── progress.tsx        # Tela de Progresso
│   │   ├── _layout.tsx             # Layout da Drawer Navigation
│   │   ├── profile.tsx             # Tela de Perfil
│   │   └── settings.tsx            # Tela de Configurações
│   ├── _layout.tsx                 # Layout da Stack Navigation (Root)
│   └── index.tsx                   # Tela de Login/Inicial
├── assets/
├── babel.config.js
├── app.json
├── package.json
└── README.md
```

## Como Executar o Projeto

1.  **Instale as dependências:**
    \`\`\`bash
    pnpm install
    # ou npm install / yarn install
    \`\`\`
2.  **Execute o projeto:**
    \`\`\`bash
    npx expo start
    \`\`\`
3.  **Use o aplicativo Expo Go** no seu celular ou um emulador para escanear o QR Code.
\`\`\`
