# Automatização de Testes e Deploy dos Relatórios no Github Pages

### 🛠 Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:

* [Postman](https://www.postman.com/)      
* [Newman](https://github.com/postmanlabs/newman)      
* [Github Actions](https://docs.github.com/pt/actions)
* [Newman Reporter HTML](https://github.com/DannyDainton/newman-reporter-htmlextra)
* [Actions Gh Pages](https://github.com/peaceiris/actions-gh-pages)

### 🚀 Organização do projeto

Este projeto é composto por 3 arquivos principais:
1. gorest.json - Arquivo gerado pelo Postman com os testes realizados
2. environment.json - Arquivo gerado pelo Postman com as váriaveis de ambiente utilizadas
3. github-ci - Arquivo com configuração de CI (instalação dos pacotes, execução dos testes e deploy do site)

💡 Para o Workflow funcionar é preciso que os nomes dos arquivos sejam iguais aos informados no github-ci (gorest.json, environment.json)

### 🎨 Layout do Relatório

<img src="https://github.com/fabioivi/qa-newman-actions-pages/blob/main/.github/images/Default_Report.gif" alt="screenshot projeto" width="800" >


### 🎲 Como utilizar este projeto

```bash
# Clone este repositório para a sua máquina
$ git clone git@github.com:fabioivi/qa-newman-actions-pages.git

# Atualize o arquivo gorest.json com o seu arquivo de testes automatizados gerado pelo Postman
$ gorest.json

# Atualize o arquivo environment.json com o seu arquivo de váriaveis de ambiente gerado pelo Postman
$ environment.json

# Clique no menu settings e depois selecione o menu Pages, na opção Source selecione a opção "Deploy from branch" e depois na opção branch escolha a opcão gh-pages

# Agora é só enviar as modificações para o github e pronto

# O servidor iniciará no link - https://seuNomeDeUsuario.github.io/qa-newman-actions-pages/
```
