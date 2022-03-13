

# Storybook - Documentação de componentes

## Dica de estudo 
Como estamos falando de uma nova forma de documentação, segue vídeo com tutorial: 

https://www.youtube.com/watch?v=5XNRCz7dcyU&list=PLBSn_5nxZ8EcJPGvVAKxO7WT70jcoj40n


## Uso

Para usar o Storybook, você precisará certificar-se de que a dependência esteja no package.json do sistema.

 
Como executar o script
---

Abra o terminal no projeto e digite:

```
npm run storybook
```

Se tudo deu certo, você conseguirá abrir o servidor do storybook na porta http://localhost:6006/ 


 ## Modo de uso
 
De forma geral, ao rodar o storybook conseguimos codar e estilizar o componente e o mesmo é renderizado automaticamente após o ```ctrl-s```.

 ## Implementação
 
O storybook possibilita a visualização dos componentes de forma complenta, isso é nele conseguimos renderizar as "n" versões de um botão, se é azul com texto branco, disable, com ou sem ícone e por ai vai.

 
```
// Importe o componente, dependencias como icones e o ComponentStory do storybook
    import { ComponentStory } from '@storybook/react';
    import { BiPlus } from 'react-icons/bi';
    import { Button } from './Button';
    
    
    export default {
       title: "Button",
       argTypes: {      
// São os args types que darão ao storybook as possibilidades de edição dos nossos componentes.
          variant: {
             options: ["primary", "secondary"],
             control: { type: "radio" },
          },
          size: {
             options: ["sm", "md", "lg"],
             control: { type: "radio" },
          },
          children: {
             type: "string"
          },
          disabled: {
             type: "boolean",
             defaultValue: false
          },
          onClick: {
             type: "function"
          },
          icon: {
             type: "function"
          },
          iconPosition: {
             options: ["start", "end"],
             control: { type: "radio" }
          }
       }
    };
// A variavel Template armazena todas as caracteristicas que poder ser usadas nos exemplos:
   const Template: ComponentStory<typeof Button> =
       ({ variant, children, onClick, disabled, size, icon, iconPosition }) => (
          <Button
             variant={variant}
             onClick={onClick}
             disabled={disabled}
             size={size}
             icon={icon}
             iconPosition={iconPosition}
          >
             {children}
          </Button>
       )
 
// Para adicionar exemplos no storybook mude os args adicionando valores que temos no Template
    
    export const Primary = Template.bind({});
    Primary.args = {
       variant: "primary",
       children: "Primary"
    };
    
    export const Secondary = Template.bind({});
    Secondary.args = {
       variant: "secondary",
       children: "Secondary"
    }
    
    export const WithIconStart = Template.bind({});
    WithIconStart.args = {
       variant: "primary",
       children: "Icon",
       icon: <BiPlus />,
       iconPosition: "start"
    }
    
    export const WithIconEnd = Template.bind({});
    WithIconEnd.args = {
       variant: "primary",
       children: "Icon",
       icon: <BiPlus />,
       iconPosition: "end"
    }

```

## Documentação

-   [Storybook](https://storybook.js.org/) 

## Duvidas

-   Manda mensagem no grupo do skype
