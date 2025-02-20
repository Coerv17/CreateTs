Criação de um novo projeto

```jsx
npm init -y
```

Instalar o typescript e node como dependência de desenvolvimento

```jsx
npm install typescript @types/node -D
```

criar o package.json

```jsx
npx tsc --init
```

acessar o link para poder modificar o tsconfig

https://github.com/microsoft/TypeScript/wiki/Node-Target-Mapping

modificar e deixar a config assim

```jsx
Node 20
{
  "compilerOptions": {
    "lib": ["ES2023"],
    "module": "node16",
    "target": "ES2023"
  }
}
```

Baixar o tsx parecido o nodemon

```jsx
npm install tsx -D
```

depois ir no package.json e modificar o scripts 

```jsx
"dev":"tsx watch src/index.ts" --passar o caminho do codigo
"dev": "tsx watch --env-file .env src/index.ts" -- passar tambem isso para rodar o .env sem precisar do dotenv, precisa reneicar o terminal para funcionar
```

finalizando

```jsx
npm run dev
```
