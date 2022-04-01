
<h1 align="center">
  Qarentena-front-web-ruby
</h1>

# Indice
- [Sobre](#-sobre)
- [Tecnologias utilizadas](#-tecnologias-utilizadas)
- [Como baixar o projeto](#-como-baixar-o-projeto)

## 👀 Sobre

Curso com o principal objetivo de automatizar alguns cenários de testes de cadastro.

---

## 💻 Tecnologias utilizadas

Foram utilizadas as seguintes tecnologias:

- [Ruby](https://www.ruby-lang.org/pt/)
- [Capybara](https://github.com/teamcapybara/capybara)
- [Cucumber](https://cucumber.io/)

---

## Como baixar o projeto 

Siga os seguintes passos para baixar o arquivo:

Fazer o clone do projeto
Abrir a pasta no VSCode
Abrir o terminal (do VSCode, ou o da sua preferência e navegar até a pasta do projeto) e rodar o comando 'bundle install'
Para rodar os cenários, utilizar o comando de run do Cucumber: ex.:
rodar todos os cenários: 'cucumber'

rodar uma feature: cucumber features/specs/01-cadastro_fixo.feature

rodar um cenário pela tag: cucumber -t @cadastro_valido_fixo_pf

rodar todos os cenários por tag: cucumber -t @regressivo

Roteiro para RECRIAR o projeto:

Abrir uma pasta vazia no VSCode
Criar o arquivo Gemfile (sem extensão) e incluir:
source 'https://rubygems.org'

gem 'capybara' gem 'cucumber' (gem 'cucumber', '~> 3.1.0') gem 'rspec' gem 'selenium-webdriver' gem 'site_prism' gem 'cpf_faker' gem 'faker'

Abrir o terminal (do VSCode, ou o da sua preferência e navegar até a pasta do projeto) e rodar o comando 'bundle install'
Rodar o comando 'cucumber --init'

Extras:
Configurações do driver no arquivo env.rb
para configurar o relatório do cucumber, criar o arquivo cucumber.yml na pasta raiz
As pages devem estender de SitePrism:Page para utilizar os recursos do SitePrism
