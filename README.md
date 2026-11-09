# Sistema Musical - Catálogo de Artistas e Músicas

Projeto desenvolvido para a unidade curricular de Linguagem de Marcação (LIMA), integrante do 2º semestre do curso Técnico em Desenvolvimento de Sistemas do SENAI-SP.

O objetivo do projeto é a construção da interface front-end (Sprint 1) de um sistema de catálogo digital para gerenciamento de artistas e suas respectivas obras musicais.

## Visão Geral do Projeto

A aplicação foi desenvolvida utilizando HTML5 e CSS3 puros, sem o uso de frameworks CSS, priorizando a estruturação semântica, acessibilidade básica e estilização modular com variáveis CSS.

O sistema simula um catálogo completo com fluxo de navegação entre cinco telas:
1. **Login (`login.html`)**: Tela de acesso inicial com centralização em Flexbox, validação de campos obrigatórios e dica visual de credenciais para testes.
2. **Menu Principal (`index.html`)**: Painel central de navegação construído com CSS Grid responsivo (`auto-fit`), contendo cartões clicáveis para acesso às demais áreas do sistema e botão de saída no topo.
3. **Cadastro de Artistas (`cadastro_artista.html`)**: Formulário em grade de duas colunas para registro do criador (nome, gênero musical, país e upload de foto), acompanhado da tabela de artistas cadastrados com ações de edição, exclusão e atalho para cadastro de músicas.
4. **Cadastro de Músicas (`cadastro_musica.html`)**: Formulário para inclusão de obras vinculadas a um artista (associação via campo select), campos para título, álbum, gênero, URL do YouTube, imagem de capa e área expandida (`grid-column: 1 / -1`) para a letra da música.
5. **Biblioteca Musical (`listagem_musicas.html`)**: Interface de consulta com barra de filtros (busca geral por texto, filtro por artista e filtro por gênero) e tabela com a listagem completa das obras, link externo para o vídeo no YouTube e botões de gerenciamento.

## Tecnologias e Recursos Utilizados

- **HTML5**: Semântica de marcação (`header`, `form`, `table`, `thead`, `tbody`, `select`, `textarea`, `input` do tipo `text`, `password`, `url` e `file`).
- **CSS3 Puro**:
  - Variáveis CSS no bloco `:root` para centralização da paleta de cores, tipografia, espaçamentos e raio de borda.
  - Reset global com `box-sizing: border-box`.
  - Layouts dinâmicos construídos com Flexbox (para alinhamentos, barras de topo, grupos de botões e centralização de telas) e CSS Grid (para a grade de formulários de 2 colunas e distribuição dos cartões do menu).
  - Estilização de estados interativos (`:hover`, `:focus`).
  - Responsividade com Media Queries (`@media (max-width: 768px)`), garantindo a transição de formulários de duas colunas para coluna única, filtros empilhados e rolagem horizontal em tabelas no celular.
