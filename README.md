# Dialoqbase

Dialoqbase is a web application that allows you to create custom chatbots with your own knowledge base. It currently supports the OpenAI API, with plans to add more language models in the future.

Here's a demo of how it works:


[![DialoqBase Demo](https://img.youtube.com/vi/Kktfs8JI4yI/0.jpg)](https://www.youtube.com/watch?v=Kktfs8JI4yI)

## Installation

1. Clone the repository and navigate to the docker directory:

```bash
git clone https://github.com/n4ze3m/dialoqbase.git
cd dialoqbase/docker
```

2. Edit the `imp.env` file and set the following environment variables:

- On Linux:

```bash
nano imp.env
```
or 

```bash
vim imp.env
```

- On Windows:

```bash
notepad imp.env
```


Set the `OPENAI_API_KEY` variable to your OpenAI API key. You can obtain an API key [here](https://platform.openai.com/account/api-keys)


3. Run the docker-compose file:

```bash
docker-compose up -d
```

or

```bash
docker compose up -d
```

4. Open your browser and go to `http://localhost:3000`.

5. Log in using the default credentials:

```bash
username: admin
password: admin
```

_Important: After the first login, remember to change the default credentials._

## Features

- Create custom chatbots with your own knowledge base 

- Utilize powerful language models to generate responses 

- Utilize PostgreSQL for vector search and storing the knowledge base (eliminating the need for an additional vector database)

## Stack

- [React](https://reactjs.org/)
- [Node.js](https://nodejs.org/)
- [Fastify](https://www.fastify.io/)
- [LangChain](https://langchain.com/)
- [PostgreSQL](https://www.postgresql.org/)
- [Redis](https://redis.io/)

## Disclaimer

Dialoqbase is a side project and is not ready for production. It is still in the early stages of development and may contain bugs and security issues. Use it at your own risk. *Breaking changes may occur at any time without prior notice.*

## TODO


- [ ] Add more LLMs both free and paid

- [ ] Add more dataloaders

- [ ] Support other embedding models

- [ ] Fix the UI issues

- [ ] Add more features


## License

[MIT](LICENSE)