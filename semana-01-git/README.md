# 📚 Semana 01 - Git e GitHub

Esse diretório contém a documentação técnica e os principais aprendizados práticos adquiridos durante a primeira semana da capacitação da Asimov Jr. O foco desta etapa foi o domínio de versionamento de código, estruturação de repositórios e boas práticas de commits.

## 🛠️ Comandos Essenciais do Git

Durante a criação do perfil e organização do projeto, o fluxo contínuo de versionamento foi mantido através dos seguintes comandos básicos:

* **`git init`**: Inicializa um novo repositório Git local.
* **`git status`**: Inspeciona o estado atual dos arquivos (modificados, na área de staging ou não rastreados).
* **`git add <arquivo>`**: Prepara alterações específicas para o próximo commit. O uso de `git add .` envia todas as modificações de uma vez para a *staging area*.
* **`git commit -m "mensagem"`**: Empacota as alterações preparadas no histórico local com uma mensagem descritiva.
* **`git push`**: Envia os commits locais para o servidor remoto (GitHub). Na primeira vez em uma nova branch, utiliza-se `git push -u origin <nome-da-branch>` para criar o vínculo.
* **`git checkout <branch>`**: Alterna entre ramificações (branches) do projeto.
* **`git merge <branch>`**: Integra as alterações de uma branch específica para dentro da branch atual em que se está trabalhando.

---

## 🏷️ Padrão Conventional Commits

Para manter o histórico do repositório legível, rastreável e profissional, todas as atualizações seguiram o padrão *Conventional Commits*. 

Abaixo estão os tipos utilizados na prática durante esta semana:

| Tipo | Aplicação | Exemplo de Uso no Projeto |
| :--- | :--- | :--- |
| **`docs`** | Alterações exclusivas em arquivos de documentação (como o `README.md`). | `docs: adiciona curriculo completo e estilizado` |
| **`fix`** | Correções de bugs, links quebrados ou falhas estruturais. | `fix: corrige links e formatação do readme` |
| **`feat`** | Adição de novas funcionalidades, arquivos base ou pastas. | `feat: adiciona gitignore e estrutura de pastas` |


---

## 🔀 Resolução do Conflito de Merge
Para cumprir os requisitos da semana, provoquei intencionalmente um conflito alterando a mesma linha do `README.md` principal em duas branches distintas (`main` e `semana-01-git`). Ao executar `git merge main` na minha branch de trabalho, o Git acusou o conflito. Utilizei o VS Code para inspecionar os marcadores de colisão (`<<<<<<<`, `=======`), selecionei a opção "Accept Current Change" para manter o currículo correto, limpei os resquícios e finalizei a integração com um novo commit.

---

## 🚀 Principais Atividades Realizadas

- [x] Construção de um `README.md` principal estilizado, com apresentação pessoal, badges e painel de estatísticas dinâmico.
- [x] Configuração do arquivo `.gitignore` para evitar o rastreamento de arquivos de sistema e pastas não desejadas.
- [x] Uso de ramificações (branches) para isolar o desenvolvimento da semana 01.
- [x] Simulação e resolução de conflito de *merge* via terminal e VS Code.
- [x] Realização de Pull Request (PR) documentado para integrar a branch à `main`.