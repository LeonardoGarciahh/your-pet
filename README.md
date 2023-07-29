# Your-Pet: Plataforma para Localizar Locais Pet Friendly
# Descrição
O Your-Pet é uma plataforma desenvolvida com o objetivo de auxiliar tutores de animais de estimação a encontrarem locais e empresas pet friendly. Com a crescente integração dos animais de estimação ao convívio familiar, é essencial que os tutores possam localizar facilmente estabelecimentos que permitam a presença de seus pets, proporcionando momentos de lazer e interação entre ambos.

# Equipe:

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/GiorgioFL15">
        <img src="https://github.com/GiorgioFL15.png" width="100px" height="100px" alt="GiorgioFL15">
        <br />
        <sub><b>Giorgio Frigotto</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/ivorybr">
        <img src="https://github.com/ivorybr.png" width="100px" height="100px" alt="ivorybr">
        <br />
        <sub><b>Ivo Ramos</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/LeonardoGarciah">
        <img src="https://github.com/LeonardoGarciah.png" width="100px" height="100px" alt="LeonardoGarciah">
        <br />
        <sub><b>Leonardo Garcia</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/thiagomeneguzzi">
        <img src="https://github.com/thiagomeneguzzi.png" width="100px" height="100px" alt="thiagomeneguzzi">
        <br />
        <sub><b>Thiago Meneguzzi</b></sub>
      </a>
    </td>
    <!-- Adicione mais colunas conforme necessário para cada contribuidor -->
  </tr>
</table>

# Funcionalidades
A plataforma Your-Pet oferece as seguintes funcionalidades:

- Localização de Estabelecimentos Pet Friendly: Os usuários podem pesquisar por locais, como restaurantes, cafés, parques, hotéis e outros estabelecimentos, que aceitam animais de estimação. A busca pode ser filtrada por tipo de local, raio de distancia e outros critérios.

- Avaliações e Comentários: Os usuários podem deixar avaliações e comentários sobre os estabelecimentos que visitaram com seus pets. Essa funcionalidade permite que outros tutores tenham insights sobre a qualidade do atendimento e da experiência pet friendly oferecida por cada local.

- Cadastro de Empresas Pet Friendly: Estabelecimentos e empresas interessados em serem listados como pet friendly podem se cadastrar na plataforma. Após uma verificação, suas informações serão disponibilizadas para os usuários da plataforma.

- Informações Detalhadas: Cada estabelecimento listado possui uma página com informações detalhadas sobre suas políticas pet friendly, horários de funcionamento, localização, entre outras informações relevantes.

- Integração com Mapas: A plataforma utiliza o Leaflet para a visualização de mapas, permitindo que os usuários visualizem a localização dos estabelecimentos.

- Perfil do Cliente: Os tutores podem criar perfis personalizados na plataforma, e interajir com os perfis empresas, como, avaliar, curtir e comentar postagens.

- Perfil da Empresa: As empresas pet friendly possuem perfis próprios na plataforma, onde podem fornecer informações detalhadas sobre o estabelecimento, como uma descrição, horários de funcionamento, serviços oferecidos e outras comodidades. Além disso, elas podem realizar postagens, divulgando eventos, descontos especiais ou novidades relacionadas ao universo pet.

# Tecnologias Utilizadas
O sistema Your-Pet foi desenvolvido utilizando as seguintes tecnologias:

- Front-end: ReactJS, Leaflet (para mapas), Material-UI (Design System), HTML5, CSS3.
- Back-end: Python, FastAPI (framework web), SQLAlchemy (ORM - Object-Relational Mapping).
- Banco de Dados: PostgreSQL (ou outra opção compatível).
- Autenticação e Armazenamento de Imagens: Firebase (Firebase Auth e Firebase Storage).
- Hospedagem: Front-end hospeado na vercel e back-end na Okteto. Back-end será migrado para vercel posteriormente

# Abaixo está a estrutura de pasta atualizada do front-end do projeto:

```
  src/
  |-- App.css
  |-- App.tsx
  |-- main.tsx
  |-- application/
  |   |-- actions/
  |   |   |-- auth
  |   |   |  |-- use-cases/
  |   |   |  |  |-- test/
  |   |   |  |  |  |-- loginUseCase.test.ts
  |   |   |  |  |-- loginUseCase.ts
  |   |   |  |  |-- loginUseCaseDomain.ts
  |   |   |  |-- authActions.ts
  |   |   |  |-- authActionsDomain.ts
  |   |   | ...
  |   |-- services/
  |   |   |-- dateService/
  |   |   |  |-- test/
  |   |   |  |  |-- dateService.test.ts
  |   |   |  |-- dateService.ts
  |   |   |  |-- dateServiceDomain.ts
  |   |   | ...
  |-- components/
  |   |-- Button/
  |   |   |-- Button.tsx
  |   |   |-- styles.ts
  |   |-- ...
  |-- domain/
  |   |-- comment.tsx
  |   |-- ...
  |-- hooks/
  |   |-- useRefresh.tsx
  |   |-- ...
  |-- lib/
  |   |-- styled-components.ts
  |   |-- ...
  |-- Router/
  |   |-- Router.tsx
  |-- pages/
  |   |-- Home.tsx
  |   |-- ...
  |-- screens/
  |   |-- private/
  |   |   |-- Home/
  |   |   |  |-- Home.tsx
  |   |   |  |-- styles.ts
  |   |-- public/
  |   |   |-- Login/
  |   |   |  |-- Login.tsx
  |   |   |  |-- styles.ts
  |-- utils/
  |   |-- validators/
  |   |   |-- validators.ts
  |   |   |-- validatorsDomain.ts
  |   |-- ...
```

# Explicação da estrutura:

- App.css: Arquivo de estilos globais do aplicativo.
- App.tsx: Arquivo principal do aplicativo, onde é definida a estrutura geral da aplicação.
- main.tsx: Arquivo de inicialização do aplicativo.
- application: Pasta que contém a lógica de aplicação do sistema.
- actions: Pasta que contém as ações da aplicação, como lógica de autenticação, requisições HTTP, etc.
- services: Pasta que contém os serviços da aplicação, como funções auxiliares, formatação de data, etc.
- components: Pasta que contém os componentes reutilizáveis do aplicativo, como botões, campos de entrada, etc.
- domain: Pasta que contém as definições de domínio da aplicação, como interfaces de comentários, etc.
- hooks: Pasta que contém os hooks personalizados do aplicativo, que podem ser utilizados para compartilhar lógica entre componentes.
- lib: Pasta que contém arquivos de configuração e exportação de bibliotecas externas.
- Router: Pasta que contém o componente de roteamento do aplicativo.
- pages: Pasta que contém as páginas do aplicativo, que são renderizadas em rotas específicas.
- screens: Pasta que contém as telas do aplicativo, que utilizam componentes e podem conter estilos e lógica de negócios específicos.
- utils: Pasta que contém funções utilitárias, como validadores, entre outras.

# Abaixo está a estrutura de arquitetura do back-end do projeto:

```
root/
|-- main.py
|-- config.py
|-- auth/
|   |-- auth.py
|   |-- deps.py
|-- database/
|   |-- connection.py
|   |-- models.py
|   |-- create_db.py
|   |-- schemas.py
|-- routes/
|   |-- router_address.py
|   |-- ....
|-- your_pet/
|   |-- address.py
|   |-- ....
|-- tests/
|   |-- test_adress
|   |   |-- __init__.py
|   |   |-- test_address.py

```

# Explicação da estrutura:

- main.py: Arquivo principal para inicializar o servidor da aplicação.
- config.py: Arquivo para configurações e inicializações de variáveis de ambiente.
- auth: Pasta que contém os arquivos relacionados à autenticação e autorização de usuários.
- auth.py: Arquivo com funções para verificar a autenticação do usuário e gerar tokens de acesso.
- deps.py: Arquivo com dependências e configurações de autenticação.
- database: Pasta que contém os arquivos relacionados ao banco de dados e modelos ORM.
- connection.py: Arquivo com a conexão e configurações do banco de dados PostgreSQL.
- models.py: Arquivo com as definições dos modelos ORM do banco de dados.
- create_db.py: Arquivo com a lógica para criar o banco de dados e tabelas.
- schemas.py: Arquivo com os esquemas de validação e serialização de dados.
- routes: Pasta que contém os arquivos das rotas da API, organizados por entidade ou tabela do banco de dados.
- router_address.py: Arquivo que define as rotas relacionadas à entidade "Address".
- your_pet: Pasta que contém a lógica das rotas da API, organizada por entidade ou tabela do banco de dados.
- address.py: Arquivo que contém a lógica relacionada à entidade "Address".
- tests: Pasta que contém os testes das rotas da API, organizados por entidade ou tabela do banco de dados.
- test_address: Pasta que contém os testes relacionados à entidade "Address".
- init.py: Arquivo para marcar a pasta como um pacote de testes.
- test_address.py: Arquivo com os casos de teste específicos para a entidade "Address".
