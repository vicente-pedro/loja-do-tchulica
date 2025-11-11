# 🛒 Loja do Tchulica

E-commerce moderno de smartphones e acessórios desenvolvido com **Vite + React + TypeScript**.

## 🎨 Cores da Marca
- **Amarelo**: `#FFD700` (principal)
- **Preto**: `#000000` (secundária)
- **Laranja**: `#FFA500` (destaque)

## 🚀 Tecnologias Utilizadas

- **Vite** - Build tool moderna e rápida
- **React 18** - Biblioteca para interfaces
- **TypeScript** - Tipagem estática
- **React Router DOM** - Navegação entre páginas
- **Context API** - Gerenciamento de estado do carrinho

## 📁 Estrutura do Projeto

```
loja-do-tchulica/
├── src/
│   ├── components/        # Componentes reutilizáveis
│   │   ├── Header.tsx
│   │   ├── Header.css
│   │   ├── Footer.tsx
│   │   ├── Footer.css
│   │   ├── ProductCard.tsx
│   │   └── ProductCard.css
│   ├── pages/            # Páginas da aplicação
│   │   ├── Home.tsx
│   │   ├── Home.css
│   │   ├── Products.tsx
│   │   ├── Products.css
│   │   ├── ProductDetail.tsx
│   │   ├── ProductDetail.css
│   │   ├── Cart.tsx
│   │   └── Cart.css
│   ├── context/          # Context API
│   │   └── CartContext.tsx
│   ├── types/            # Tipos TypeScript
│   │   └── index.ts
│   ├── data/             # Dados mockados
│   │   └── products.ts
│   ├── App.tsx           # Componente principal
│   ├── App.css
│   ├── main.tsx          # Entry point
│   └── index.css
├── package.json
├── tsconfig.json
├── vite.config.ts
└── README.md
```

## ✨ Funcionalidades

### Páginas Implementadas
- **Home** (`/`) - Página inicial com produtos em destaque
- **Produtos** (`/produtos`) - Catálogo completo com filtros e ordenação
- **Detalhes do Produto** (`/produto/:id`) - Página individual do produto
- **Carrinho** (`/carrinho`) - Gerenciamento do carrinho de compras

### Recursos
- ✅ Listagem de produtos (smartphones e acessórios)
- ✅ Filtros por categoria
- ✅ Busca de produtos
- ✅ Ordenação (preço, nome)
- ✅ Adicionar/remover produtos do carrinho
- ✅ Controle de quantidade no carrinho
- ✅ Cálculo automático de totais
- ✅ Design responsivo (mobile-first)
- ✅ Navegação entre páginas
- ✅ Gerenciamento de estado com Context API

## 🛠️ Instalação e Execução

### Pré-requisitos
- Node.js (versão 16 ou superior)
- npm ou yarn

### Passos

1. **Clone ou baixe o projeto**
```bash
cd loja-do-tchulica
```

2. **Instale as dependências**
```bash
npm install
```

3. **Execute o projeto em modo desenvolvimento**
```bash
npm run dev
```

4. **Acesse no navegador**
```
http://localhost:5173
```

## 📦 Scripts Disponíveis

```bash
npm run dev        # Executa em modo desenvolvimento
npm run build      # Cria build de produção
npm run preview    # Visualiza o build de produção
npm run lint       # Executa o linter
```

## 🎯 Próximas Implementações (Backend)

Para adicionar backend ao projeto, você pode:

1. **API REST com Node.js + Express**
   - Criar endpoints para produtos
   - Sistema de autenticação
   - Gerenciamento de pedidos

2. **Banco de Dados**
   - MongoDB ou PostgreSQL
   - Armazenar produtos, usuários e pedidos

3. **Integração de Pagamento**
   - Mercado Pago
   - PagSeguro
   - Stripe

4. **Upload de Imagens**
   - Cloudinary
   - AWS S3

## 📝 Estrutura de Dados

### Product
```typescript
interface Product {
  id: number;
  name: string;
  category: 'smartphone' | 'acessorio';
  price: number;
  image: string;
  description: string;
  stock: number;
}
```

### CartItem
```typescript
interface CartItem extends Product {
  quantity: number;
}
```

## 🎨 Personalização

### Alterar Cores
Edite as cores nos arquivos CSS:
- `#FFD700` - Amarelo principal
- `#000000` - Preto
- `#FFA500` - Laranja para hover

### Adicionar Produtos
Edite o arquivo `src/data/products.ts` e adicione novos produtos ao array.

### Modificar Layout
Os componentes estão em `src/components/` e as páginas em `src/pages/`.

## 📱 Responsividade

O site é totalmente responsivo e funciona em:
- 📱 Smartphones (320px+)
- 📱 Tablets (768px+)
- 💻 Desktops (1024px+)

## 🤝 Contribuindo

Este é um projeto acadêmico. Sinta-se à vontade para:
1. Fazer um fork
2. Criar uma branch para sua feature
3. Fazer commit das mudanças
4. Fazer push para a branch
5. Abrir um Pull Request

## 📄 Licença

Este projeto foi desenvolvido para fins educacionais.

## 👨‍💻 Autor

Desenvolvido para o projeto da faculdade - **Loja do Tchulica**

---

**Nota**: Este é um projeto frontend. Para funcionalidade completa de e-commerce, será necessário implementar um backend com API REST, banco de dados e sistema de pagamentos.
