# API Star Tech (JSON Server)

Bem-vindo ao repositório da API temporária do projeto **Star Tech**, hospedada no JSON Server e deployada no Vercel. Esta API foi criada para suportar o front-end da aplicação desenvolvida durante a Residência Tecnológica do Porto Digital, como parte de um desafio acadêmico.

- [Repositório Front-End](https://github.com/dominuuus/Star-Tech)
- [startechdev.vercel.app](https://startechdev.vercel.app)

## Sobre o Projeto Star Tech

O projeto **Star Tech** foi desenvolvido por alunos do curso de **Análise e Desenvolvimento de Sistemas (ADS)** da **Faculdade Senac PE**, durante a **Residência Tecnológica do Porto Digital**, em 2025. O desafio foi proposto pelo **Banco do Brasil** com o objetivo de resolver o problema da elevada quantidade acumulada de pequenos problemas nos softwares, que torna o sistema mais complexo, dificulta a manutenção e reduz a produtividade da equipe.

A solução proposta é uma plataforma com **gamificação de temática espacial**, onde:
- As **missões** (tarefas de correção de bugs ou melhorias) são apresentadas por prioridade.
- As equipes ganham **recompensas** ao melhorar o sistema, promovendo qualidade, colaboração e engajamento contínuo.

### Tecnologias Utilizadas
O foco do desafio era desenvolver a solução apenas no **front-end**, utilizando as seguintes tecnologias:
- **React** (v19): Para construção da interface.
- **Vite** (v6): Para o ambiente de desenvolvimento e build.
- **TypeScript** (v5): Para tipagem estática.
- **Styled Components** (v6): Para estilização.

Para simular o back-end e consumir os dados necessários na plataforma, utilizamos o **JSON Server** para hospedar uma estrutura em JSON e integrá-la à aplicação.

## Sobre a API (JSON Server)

O **JSON Server** foi utilizado para criar uma API REST falsa, permitindo que o front-end da aplicação Star Tech consumisse dados dinamicamente durante o desenvolvimento. A API foi hospedada no **Vercel** para facilitar o acesso e a integração.

### Estrutura da API
A estrutura da API foi baseada no template criado por **Kit Loong** ([GitHub: @kitloong](https://github.com/kitloong)). Este template já inclui todas as configurações necessárias para que os endpoints sejam consumidos diretamente pelo front-end, com suporte a operações de leitura (GET) por padrão.

Abaixo está um exemplo da estrutura padrão do arquivo `db.json`, que define os dados disponíveis na API:

```json
{
  "posts": [
    { "id": 1, "title": "json-server", "author": "typicode" }
  ],
  "comments": [
    { "id": 1, "body": "some comment", "postId": 1 }
  ],
  "profile": { "name": "typicode" }
}
```

### Endpoint da API
A API está hospedada no Vercel e pode ser acessada pelo seguinte link:

- [https://bbgame-api-wine.vercel.app](https://bbgame-api-wine.vercel.app)

Exemplo de endpoints:
- `GET /missoes`: Retorna a lista de missoes.
- `GET /missoes/id`: Retornar uma missão específica através do id.
- `GET /mascotes`: Retorna a lista dos mascotes cadastrados na plataforma.


### Operações de Escrita
Por padrão, o JSON Server permite apenas operações de leitura (GET). No entanto, graças à contribuição de `@VicAv99` (issue #6 no repositório original), é possível habilitar operações de escrita (POST, PUT, DELETE). Para mais detalhes, consulte o arquivo `api/server.js` no repositório original de Kit Loong.

### Deploy no Vercel
O deploy da API foi realizado utilizando o guia **Deploy JSON Server to Vercel**, disponibilizado no template de Kit Loong. O repositório foi configurado e hospedado no Vercel, garantindo acesso contínuo durante o desenvolvimento do projeto.

## Créditos
- **Estrutura do JSON Server**: Criada por **Kit Loong** ([GitHub: @kitloong](https://github.com/kitloong)). Agradecemos pelo template e pela facilidade de configuração.
- **JSON Server**: Desenvolvido por [typicode](https://github.com/typicode/json-server).
- **Deploy**: Hospedado no [Vercel](https://vercel.com).

## Referências
- [JSON Server](https://github.com/typicode/json-server) – Documentação oficial.
- [Vercel](https://vercel.com) – Plataforma de hospedagem.
- [Deploy JSON Server to Vercel](https://shadowsmith.com/how-to-deploy-an-express-api-to-vercel) – Guia de deploy.

## Licenças
Este projeto é um trabalho acadêmico desenvolvido pelo grupo Squad 9 BB RiseUP - Residência Tecnológica do Porto Digital e está licenciado sob a [MIT License](https://opensource.org/licenses/MIT). Para uso comercial ou distribuição em larga escala, solicitamos contato prévio com os autores.

A estrutura do JSON Server segue a licença do repositório original de Kit Loong (MIT). Consulte as licenças das dependências para mais detalhes.
