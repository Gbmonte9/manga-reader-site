# Roteamento - React Router

```js
<Route path="/" element={<Home />} />
<Route path="/login" element={<Login />} />
<Route path="/manga/:id" element={<DetalhesManga />} />
<Route path="/capitulo/:id" element={<Leitor />} />
<Route path="/favoritos" element={<Favoritos />} />
```

### Rotas protegidas:

/favoritos, /perfil exigem token JWT