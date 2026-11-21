# Evidências da Frente 4 — C3

Este diretório contém saídas integrais dos testes locais repetidos na candidata `923ab5acf7dfe3f11aa7127d376e90cae7c95821`, além das capturas do site público usadas no documento `docs/EVIDENCIAS_C3_FRENTE4.docx`.

| Arquivo | O que comprova | Limite |
|---|---|---|
| `run-info-923ab5a-2026-11-21.txt` | Hash da candidata, horário e códigos de saída 0 dos três comandos | Não identifica o commit servido no Render |
| `pytest-923ab5a-2026-11-21-rerun.txt` | Pytest local: 50 aprovados, 1 ignorado, 61 avisos | O teste PostgreSQL foi ignorado; não comprova banco PostgreSQL |
| `pytest-f41-cenarios-2026-11-21.txt` | Seis cenários F41 aprovados isoladamente com API local, SQLite e mocks | Não comprova o comportamento da versão publicada |
| `vitest-923ab5a-2026-11-21-rerun.txt` | Vitest local: 17 aprovados em 3 arquivos | Os fluxos que dependem de API foram simulados |
| `vite-build-923ab5a-2026-11-21-rerun.txt` | Build de produção do Vite concluído | Build da candidata local, não do deploy público |
| `public-login-vazio-2026-11-21.png` | Mensagens de validação para login sem campos | Navegador headless; URL pública |
| `public-login-rejeitado-2026-11-21.png` | Rejeição de tentativa com credenciais sintéticas | Não prova hash do deploy |
| `public-cadastro-vazio-2026-11-21.png` | Campos obrigatórios no cadastro; formulário não enviado | Não foi criada conta nesta verificação |
| `public-groq-smoke-2026-11-21.webp` | Resultado visível da única análise sintética real via Groq | Não mostra a entrada completa nem o commit servido |

As capturas PNG foram feitas em 21/11/2026, Chromium headless, viewport 1440 × 1000. A análise real via Groq foi feita anteriormente, uma única vez; não foi repetida nem contabilizada como avaliação em lote.
