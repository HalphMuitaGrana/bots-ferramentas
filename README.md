# bots-ferramentas

Arquivos de ferramentas que o app **Bots** baixa sob demanda. Este repositório é público
só porque o app precisa baixar estes arquivos sem login; o código do app fica num repositório privado.

## agent-browser 0.36.0-omb.1 (Windows x64)

O navegador que os bots usam é o [agent-browser](https://github.com/vercel-labs/agent-browser), da
Vercel Labs (licença Apache-2.0).

- **Origem desta cópia:** a versão consertada para Windows publicada pelo projeto OpenMausBot em
  `milind-soni/OpenMausBot`, release `browser-engine-v0.36.0-omb.1`.
  - Ela parte do commit `eb05921bad874cd2a1b4fa5d1149f1ed26576cae` do agent-browser e leva o conserto
    de saída padrão no Windows do [PR #1781](https://github.com/vercel-labs/agent-browser/pull/1781),
    que a versão oficial ainda não traz.
- **Impressão digital (SHA-256)** de `agent-browser-win32-x64-0.36.0-omb.1.exe`:
  `33bee834f6a6072ec8688b0914726e0262874d758f69f27e8baf7eaac6b5ed15`.
  É o mesmo arquivo, byte a byte. O app recusa qualquer arquivo com outra impressão digital.
- **Junto vão:** as licenças (`agent-browser-LICENSE.txt` e as do axe-core), o patch aplicado
  (`agent-browser-windows-stdio.patch`), a procedência (`provenance.json`) e o README original.
- **Plano:** quando a Vercel publicar uma versão oficial com esse conserto, o app passa a baixar a
  versão oficial e esta cópia deixa de ser usada.
