
<p align="center">
  <a href="https://example.com/">
    <img src="https://dev.azure.com/tecnologiaunica/eeb30c7b-f486-43c5-a03c-31da416dae86/_apis/git/repositories/14f1cbb2-da60-4716-ae72-448e3ec0dc35/items?path=/src/assets/images/logo.png&versionDescriptor%5BversionOptions%5D=0&versionDescriptor%5BversionType%5D=0&versionDescriptor%5Bversion%5D=development&resolveLfs=true&%24format=octetStream&api-version=5.0" alt="Logo"  height=72>
  </a>
  <h3 align="center">Opti Marketing | Pasta /hooks</h3>
   </p> 
Aqui armazenamos nossos hooks. 

#### O que são ?

Quando você tem uma lógica de componente que precisa ser usada por vários componentes, podemos extrair essa lógica para um Hook customizado.

### File Tree

```bash
├─useDebounce.ts
├─useRedux.ts
└─useScreenSize.ts
```

 `useDebounce.ts`
É um hook que o usamos para criar um delay nas requisições de inputs.

 `useRedux.ts`
É um hook que facilita o gerenciamento de estado do redux.

 `useScreenSize.ts`
É um custom hook com o tamanho das telas de dispositivos ao qual nosso projeto deve estar responsivo.
