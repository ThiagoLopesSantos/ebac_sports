# Exercicio prático EBAC - Projeto de Prática com Redux Toolkit + RTK Query

Este projeto é uma loja virtual fictícia, desenvolvida como prática para consolidar conceitos de **Redux Toolkit**, **Redux Toolkit Query (RTK Query)** e integração com React. Durante o desenvolvimento, migrei o gerenciamento de estado com `useState` para uma abordagem mais robusta usando Redux, além de consumir uma API externa com RTK Query.

---

## 🚀 Tecnologias e Ferramentas

- React
- TypeScript
- Redux Toolkit
- Redux Toolkit Query (RTK Query)
- Styled Components

---

## 📚 O que foi feito e aprendido

### ✅ 1. **Refatoração do estado global**

- Substituí o uso de `useState` no `App.tsx` por gerenciamento com Redux Toolkit.
- Criei dois `slices`: um para o **carrinho** e outro para os **favoritos**.
- Com isso, centralizei o estado e deixei os componentes mais limpos e desacoplados.

### ✅ 2. **Uso do Redux Toolkit**

- Usei `createSlice()` para definir o estado e as actions do carrinho e favoritos.
- Configurei a `store` com `configureStore()`.
- Apliquei `useSelector` para acessar os estados no Redux.
- Usei `useDispatch` para disparar ações (como adicionar/remover item).

### ✅ 3. **RTK Query (Redux Toolkit Query)**

- Configurei a API com `createApi()` e `fetchBaseQuery()`.
- Criei um endpoint `getProdutos` para buscar os produtos da loja.
- Usei o hook `useGetProdutosQuery()` para consumir os dados na UI.

### ✅ 4. **Componentes desacoplados**

- Removi props desnecessárias (`favoritar`, `estaNosFavoritos`) e passei a acessar diretamente o Redux nos componentes.
- Tornei o componente `Produto` independente, usando `useSelector` e `useDispatch` internamente.

### ✅ 5. **Boas práticas**

- Usei `types` para definir o modelo de produto.
- Organizei o projeto em pastas: `components`, `containers`, `store`, `services`.
- Criei um código limpo e reutilizável, pronto para escalar.


