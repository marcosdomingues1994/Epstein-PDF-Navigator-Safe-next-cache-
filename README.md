Epstein PDF Navigator (Tampermonkey)

Este repositório contém um userscript para Tampermonkey criado para corrigir problemas graves de navegação nos arquivos PDF divulgados pelo DOJ no caso Epstein.

Motivação

Ao tentar analisar diretamente os arquivos oficiais, fica evidente um grande problema de UX:

a) não existe navegação entre datasets;

b) não existe navegação funcional entre arquivos;

c) vários PDFs agrupam múltiplos arquivos EFTA (bundles), quebrando qualquer lógica sequencial;

d) há gaps enormes entre arquivos, com muitas URLs inexistentes, isso torna a análise direta das fontes primárias lenta, confusa e desnecessariamente frustrante.

O que o script faz

O script adiciona uma interface simples de navegação diretamente na página dos PDFs, permitindo:

1) navegar para o próximo/anterior arquivo válido;

2) navegar entre datasets;

3) lidar corretamente com PDFs que representam múltiplos arquivos;

4) validar a existência de URLs antes de navegar (GET/FETCH);

5) cachear URLs válidas, reduzindo drasticamente o tempo de resposta após o primeiro acesso;

6) evitar varredura linear custosa em grandes gaps.

O que o script NÃO faz

- Não interpreta conteúdo dos arquivos.

- Não altera PDFs.

- Não coleta dados.

- Não faz qualquer juízo ou análise sobre o material.

- O objetivo é acesso, não interpretação.

Como usar:

Instale a extensão Tampermonkey no navegador.

Crie um novo script e cole o conteúdo do arquivo .user.js deste repositório.

Acesse qualquer PDF dos datasets do DOJ — a interface aparecerá automaticamente.

Observações

Este é um projeto simples, criado para resolver um problema real de acesso a dados públicos.
Pull requests, sugestões e melhorias são bem-vindos.
