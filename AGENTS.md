# Instruções para colaboradores

- Use a branch `main` e não crie novas branches.
- Faça commits com o Git e garanta que a *worktree* esteja limpa antes de finalizar.
- Não reescreva commits existentes.
- Após modificar `README.ipynb`, execute `python convert_ipynb_to_md_and_py.py` para gerar `README.md` e `README.py`. Inclua a saída desse comando na seção de testes do PR.
- Não altere a seção `## 2. Configurar/Instalar/usar o \`Git\` [1]` do arquivo `README.ipynb`.
- Cite arquivos e comandos no PR usando o formato `【F:caminho†Lx-Ly】` e `【chunk_id†Lx-Ly】`.
