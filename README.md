# README

Autores:
- Brenno Andrade Novais
- Caio Hideki Yamamoto Toyama
- Guilherme Conte Mendes Batista
- João Vitor Vieira Topan 
- Leonardo Monteiro Mello

Each Lab será a ferramenta web a qual irá servir como repositório colaborativo para materiais de estudo de cursos e disciplinas da EACH e fórum de dúvidas.

## 1. Medidas de Monitoramento

### CodeClimate Badges:
- [![Maintainability](https://api.codeclimate.com/v1/badges/6e3e8570979cdde31f4f/maintainability)](https://codeclimate.com/github/brenno-novais/each-lab/maintainability)
- [![Test Coverage](https://api.codeclimate.com/v1/badges/6e3e8570979cdde31f4f/test_coverage)](https://codeclimate.com/github/brenno-novais/each-lab/test_coverage)

### Github Actions Badge:
- [![GitHub Actions Demo](https://github.com/brenno-novais/each-lab/actions/workflows/github-actions-demo.yml/badge.svg)](https://github.com/brenno-novais/each-lab/actions/workflows/github-actions-demo.yml)

## 2. Links

- Heroku:

- Pivotal Tracker:

## 3. Setup

Os passos a seguir dizem respeito ao sistema operacional Ubuntu.

### Instale o rbenv (ambiente virtual para ter controle de versão Ruby)

1. Clone o rbenv na pasta ~/.rbenv:

```
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
```

2. Configure seu shell para rodar o rbenv:

```
echo 'eval "$(~/.rbenv/bin/rbenv init - bash)"' >> ~/.bashrc
```

3. Entre na pasta que pretende colocar o projeto (recomendo nova pasta) e instale a versão 3.2.2 do Ruby:

```
rbenv install 3.2.2
```

Obs: Talvez seja necessário instalar o libyaml: 
    ```
    sudo apt-get install libyaml-dev
    ```

4. Defina o a versão 3.2.2 como a versão local:

```
rbenv local 3.1.2
```

5. Instale o Rails:
```
gem install rails
```

6. Clone esse repositório e entre na pasta.

7. Instale as dependências do projeto:
```
bundle install
```

### Testes

Para os testes, rode:
```
rake spec
```

```
rake cucumber
```

É esperado uma output na tela, indicando que todos os testes passaram com sucesso.