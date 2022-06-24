# Workflow do GitHub Actions para testes de API REST, testes via chamadas HTTP com Newman + Postman, push no Github Pages

## 🚀 Organização do projeto

Este projeto é composto por 3 arquivos principais:
1. gorest.json - Arquivo gerado pelo Postman com os testes realizados
2. environment.json - Arquivo gerado pelo Postman com as váriaveis de ambiente utilizadas
3. github-ci - Arquivo com configuração de CI (instalação dos pacotes, execução dos testes e deploy do site)

💡 Para o Workflow funcionar é preciso que os nomes dos arquivos sejam iguais aos informados no github-ci (gorest.json, environment.json)

### 🎲 Como utilizar este projeto

```bash
# Clone este repositório para a sua máquina
$ git clone git@github.com:fabioivi/qa-newman-actions-pages.git

# Atualize o arquivo gorest.json com o seu arquivo de testes automatizados gerado pelo Postman
$ gorest.json

# Atualize o arquivo environment.json com o seu arquivo de váriaveis de ambiente gerado pelo Postman
$ environment.json

# Agora é só enviar as modificações para o github e pronto

# O servidor iniciará no link - https://seuNomeDeUsuario.github.io/qa-newman-actions-pages/
```
