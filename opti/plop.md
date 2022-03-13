
# Plop - Geração de componentes

## Descrição

Essa documentação demostra como criar um componente no projeto com Plop. O Plop é um lib que automatiza o chato trabalho de criar pastas e arquivos para nossos componentes.

## Criando Components com Plop
![enter image description here](https://res.cloudinary.com/dgorwmjud/image/upload/v1647124242/Documenta%C3%A7%C3%A3o%20Opti/carbon_3_hobte2.png)
 </div> 

    npm run gen Nome 
    # Substituir Nome pelo nome do componente que vai ser criado
    
    component digite: C || page digite: P
    # Atualmente temos duas automatizações para criar arquivos, a de componente e a de página, O prompt indica C para geração de Componente e P para geração de página

OBS: O nome deve ser inserido seguindo qualquer uma das seguintes formas: 

button

Button

inputText 

InputText 
 
## Por dentro de cada arquivo

  **─ Index.ts**
  
O arquivo index é o arquivo mais simples. Aqui, você simplesmente vai exportar o componente e a tipagem do mesmo para que seja mais fácil importar em outros arquivos
**├─ Name.stories.tsx**

Esse arquivo utiliza a biblioteca storybook para gerar uma documentação dinâmica para o seu componente, mas é necessário configurá-la. Existem alguns exemplo no projeto de como um storybook configurado funciona.

**├─ Name.styled.ts**
Esse arquivo é onde vai ficar a estilização do componente. Para fazer a estilização, estamos usando o styled(), do Material UI.  

**├─  Name.test.ts** 
 Neste arquivo vão se encontrar todos os testes para validar se o componente está funcionando corretamente. 

**├─  Name.tsx** 
Este arquivo é onde você vai escrever o seu componente em si 

**└─  Name.types.ts**  
Neste arquivo se encontra todas as tipagens que foram criadas por nós que foram usadas durante o componente
 
### Como implementar
Exemplo de implementação do component Button


**Index.tsx** 

![enter image description here](https://res.cloudinary.com/dgorwmjud/image/upload/v1647125872/Documenta%C3%A7%C3%A3o%20Opti/index-exports_l2aw2z.png)


**Button.tsx**


![enter image description here](https://res.cloudinary.com/dgorwmjud/image/upload/v1647126550/Documenta%C3%A7%C3%A3o%20Opti/button_component_v4db5n.png)


**Button.styled.ts** 


![enter image description here](https://res.cloudinary.com/dgorwmjud/image/upload/v1647126249/Documenta%C3%A7%C3%A3o%20Opti/styled_rhtgmn.png)


**Button.Stories.tsx** 


![enter image description here](https://res.cloudinary.com/dgorwmjud/image/upload/v1647126049/Documenta%C3%A7%C3%A3o%20Opti/stories_j4vmcj.png)
 


**Button.test.ts**


![enter image description here](https://res.cloudinary.com/dgorwmjud/image/upload/v1647126437/Documenta%C3%A7%C3%A3o%20Opti/test_xhn0gn.png)


**Button.test.tsx**


![enter image description here](https://res.cloudinary.com/dgorwmjud/image/upload/v1647126688/Documenta%C3%A7%C3%A3o%20Opti/testes_u4pzov.png)


## Documentação

-  [Plop](https://plopjs.com/) 
-  Como estamos usando o Storybook ? Leia a sessão de [Components ](https://dev.azure.com/tecnologiaunica/OptiMarketing/_wiki/wikis/wiki/69/components)

## Duvidas

-   Interessante quebrar um pouco a cabeça pesquisando no google, youtube e documentação. 
-  Após 30 minutos, manda mensagem no grupo do skype.

