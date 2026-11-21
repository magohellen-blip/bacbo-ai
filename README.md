# BAC BO AI — protótipo Android 0.1

## Construir usando somente o celular
Este projeto inclui um fluxo GitHub Actions para compilar o APK na nuvem, usando o navegador do celular.

1. Baixe e extraia o ZIP no celular.
2. No navegador, entre em https://github.com e crie uma conta ou entre.
3. Crie um repositório novo (por exemplo `bacbo-ai`).
4. Envie todos os arquivos e pastas do projeto extraído para o repositório, preservando a estrutura. Inclua a pasta oculta `.github`.
5. Abra a aba **Actions** do repositório. Se solicitado, habilite GitHub Actions.
6. O workflow **Build BAC BO AI APK** deverá iniciar após o envio. Se não iniciar, abra o workflow e toque em **Run workflow**.
7. Quando terminar com sucesso, abra a execução e baixe o artefato **BAC-BO-AI-debug**.
8. Extraia o artefato ZIP e toque em `app-debug.apk` para instalar. O Android poderá pedir autorização para instalar apps dessa origem.

## O que o protótipo faz
- Tela inicial.
- Solicita permissão de exibição sobre outros apps.
- Cria uma bolha "AI" arrastável.
- Abre um painel demonstrativo.

## O que ainda não faz
- Não captura a tela da Brasawin.
- Não tem OCR.
- Não identifica resultados reais nem gera sinais estatísticos.
- O texto de painel é apenas demonstrativo.

A etapa seguinte será desenvolver a captura autorizada via Android MediaProjection (com consentimento explícito do usuário) e o reconhecimento OCR. Se o jogo bloquear captura, não haverá tentativa de contornar esse bloqueio.
