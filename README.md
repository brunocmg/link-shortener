# Link Shortener


## Subir o banco

```bash
docker compose up -d
```

Se quiser parar o banco depois:

```bash
docker compose down
```

## Inicializar o projeto

Instale as dependências:

```bash
npm install
```

Depois rode a migration inicial do Prisma:

```bash
npm run db:migrate
```

## Rodar a API

Modo desenvolvimento:

```bash
npm run dev
```

Build e execução em produção local:

```bash
npm run build
npm start
```

## Teste rápido

Com a API no ar, confira a rota de health:

```bash
GET http://localhost:3000/health
```

Resposta esperada:

```json
{
	"status": "success",
	"message": "API link shortener is running!"
}
```