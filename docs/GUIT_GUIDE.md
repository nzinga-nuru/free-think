# GUIT Guide: Solução de Conflitos e Atualização de URL Remoto

'''
bundle exec jekyll serve --host 0.0.0.0 --port 4000
'''


## Índice

1. [Atualização de URL Remoto do Repositório](#atualização-de-url-remoto-do-repositório)
2. [Resolução de Conflitos de Mesclagem](#resolução-de-conflitos-de-mesclagem)
3. [Dicas Adicionais](#dicas-adicionais)

---

## Atualização de URL Remoto do Repositório

Quando você altera o nome do repositório no GitHub, o URL do repositório também muda. Siga os passos abaixo para atualizar o URL remoto do repositório no seu ambiente local.

### Passo a Passo

1. **Verifique a URL atual do repositório remoto:**

   ```
   bash
   git remote -v
```

O comando acima deve mostrar algo como:

```
origin  https://github.com/SEU_USUARIO/free-think (fetch)
origin  https://github.com/SEU_USUARIO/free-think (push)
```
2. Atualize o URL remoto para o novo nome do repositório:

```git remote set-url origin https://github.com/SEU_USUARIO/free-thinker

```

3. Verifique se a URL foi atualizada corretamente:

```
git remote -v
```

O comando acima deve mostrar algo como:
```origin  https://github.com/SEU_USUARIO/free-thinker (fetch)
origin  https://github.com/SEU_USUARIO/free-thinker (push)
```

4. Tente fazer o push novamente

```
git push origin main
```

## Resolução de Conflitos de Mesclagem
Quando há conflitos de mesclagem no repositório, você precisa resolvê-los manualmente antes de fazer o push. Siga os passos abaixo para resolver conflitos de mesclagem.

### Passo a Passo

1. Verifique o estado do repositório:

```git status
```

Esse comando listará os arquivos com conflitos e outros arquivos modificados.

2. Edite cada arquivo com conflito para resolver manualmente os conflitos. Os conflitos são marcados assim:

```
<<<<<<< HEAD
Seu conteúdo local
=======
Conteúdo do repositório remoto
>>>>>>> NomeDaBranchRemota
```

Escolha qual conteúdo manter (ou combine os dois) e remova os marcadores (<<<<<<<, =======, >>>>>>>).

3. Adicione os arquivos resolvidos:

```
git add nome_do_arquivo_resolvido
```
4. Finalize a mesclagem:

```git commit
```
Se a mensagem de commit não for aberta automaticamente, use:

```
git commit -m "Resolve conflitos de mesclagem"
```

5. Tente fazer o push novamente:

```
git push origin main

```

## Dicas Adicionais

- Sempre faça git pull antes de iniciar novas alterações para minimizar conflitos.
- Use git status frequentemente para monitorar o estado dos arquivos no repositório.
- Caso enfrente dificuldades em resolver conflitos, você pode usar ferramentas visuais como `gitk`, `meld` ou a interface gráfica do GitHub Desktop.
