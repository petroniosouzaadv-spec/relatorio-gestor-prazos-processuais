# Relatório do Gestor de Prazos Processuais.

Este repositório está pronto para publicação no GitHub Pages.

## Arquivos da raiz

- `index.html`
- `.nojekyll`
- `favicon.ico`
- `favicon-16x16.png`
- `favicon-32x32.png`
- `apple-touch-icon.png`
- `android-chrome-192x192.png`
- `android-chrome-512x512.png`
- `site.webmanifest`
- `README.md`
- `AUTOMACAO-LEIA.txt`

## Workflow de publicação

O arquivo de deploy está em:

`.github/workflows/deploy-pages.yml`

## Como publicar

1. Crie um repositório novo no GitHub.
2. Envie os arquivos da raiz exatamente como estão neste pacote.
3. Envie também a pasta `.github/workflows` com o arquivo `deploy-pages.yml`.
4. No GitHub, vá em `Settings > Pages`.
5. Em `Build and deployment`, selecione `GitHub Actions`.
6. Faça o commit inicial.
7. Vá em `Actions` e aguarde a execução do workflow.
8. Após concluir, o GitHub Pages vai gerar a URL pública do site.

## Atualização diária por automação

A automação deve sobrescrever somente o arquivo `index.html`.

Fluxo recomendado:
1. gerar o novo HTML do dia;
2. substituir `index.html`;
3. fazer commit;
4. fazer push para `main`.

Os demais arquivos do kit devem permanecer intactos.
