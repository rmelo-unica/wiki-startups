
<p align="center">
  <a href="https://example.com/">
    <img src="https://dev.azure.com/tecnologiaunica/eeb30c7b-f486-43c5-a03c-31da416dae86/_apis/git/repositories/14f1cbb2-da60-4716-ae72-448e3ec0dc35/items?path=/src/assets/images/logo.png&versionDescriptor%5BversionOptions%5D=0&versionDescriptor%5BversionType%5D=0&versionDescriptor%5Bversion%5D=development&resolveLfs=true&%24format=octetStream&api-version=5.0" alt="Logo"  height=72>
  </a>
  <h3 align="center">Opti Marketing | Pasta /reducers </h3>
   </p> 
Usamos reducers no projeto pra guardar estados globais (estados que conseguimos usar na aplicação inteira).

Dentro dele temos os valores, que sempre são variáveis de tipos primitivos (boolean, string, number, obj, etc). Neles temos as actions, que são funções que alteram os valores (só elas podem alterar eles);

### File Tree
```bash
reducers/
├─authentication.ts
├─blog.ts
├─index.ts
└─keyword.ts

```
 **Nossa lista de reducers**

- authentication
	- Armazena globalmente o usuario atual

- blogs 
	- Armazena globalmente os dados do projeto atual
- keywords
	- Armazena globalmente os dados de uma determinada palavra-chave


