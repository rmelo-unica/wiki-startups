<p align="center">
  <a href="https://example.com/">
    <img src="https://dev.azure.com/tecnologiaunica/eeb30c7b-f486-43c5-a03c-31da416dae86/_apis/git/repositories/14f1cbb2-da60-4716-ae72-448e3ec0dc35/items?path=/src/assets/images/logo.png&versionDescriptor%5BversionOptions%5D=0&versionDescriptor%5BversionType%5D=0&versionDescriptor%5Bversion%5D=development&resolveLfs=true&%24format=octetStream&api-version=5.0" alt="Logo"  height=72>
  </a>
  <h3 align="center">Opti Marketing | Pasta /api</h3>
   </p> 
Nela temos alguns arquivos importantes:

### File Tree
```bash
├─ controllers/
├─ models/
└─ services/
``` 

##  Detalhes importantes
No diretório `/api` temos todos os serviços que cuidam da comunicação entre a aplicação React (frontend) e a nossa API C# (backend). 

 `/controllers`
Nesse diretório criamos as funções que se comunicaram com as endpoints das controllers do backend.
 
 `/models`
Aqui tiparemos nossas entidades com typescript assim como eleas foram tipadas no backend.

  `/services`
Nosso principal serviço usa de duas ferramentas para a comunicação com os endpoints da api, elas axios e react-query.
