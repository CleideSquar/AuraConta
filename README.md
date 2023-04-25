# AuraConta

## Introdução
Este é um componente Salesforce Aura que exibe uma lista de contas que estão atualmente em negociação. O componente chama um controlador Apex para recuperar a lista de contas e as exibe usando uma iteração.

### Explicação do Código
**Controlador Apex**

O controlador Apex tem um método chamado getAccountNR que é chamado pelo componente para recuperar a lista de contas. O método retorna uma lista de registros de conta.

**Componente**

O componente possui os seguintes atributos:

**accs:** Uma matriz de registros de Account que serão exibidos.

O componente possui os seguintes manipuladores:

**init:** Um manipulador que é invocado quando o componente é inicializado. Ele chama a função doInit para recuperar a lista de contas.

O componente usa o componente **lightning:card** para exibir a lista de contas. O componente **aura:iteration** é usado para iterar através da matriz accs e exibir os registros de conta.

Os seguintes campos são exibidos para cada conta:

**Name:** O nome da conta

**Contatato__c:** Um campo personalizado no objeto Conta.

**Rating:** A classificação da conta.

### Controlador Javascript
O controlador Javascript tem uma função **doInit** que chama o método **getAccountNR** no controlador Apex para recuperar a lista de contas.

A função **getAccountNR** chama o método **c.getAccountNR** no componente para invocar o controlador Apex. A resposta é então verificada para o sucesso e os registros de conta são definidos como o atributo accs no componente.

### Como Usar
Para usar este componente, você pode clonar o repositório e implantá-lo em sua org do Salesforce. Depois de implantado, você pode adicionar o componente à sua página Lightning.

**Obs.:** Certifique-se de atualizar o atributo controller no componente para apontar para o controlador Apex correto.

# Lista de Exercício: Aura - A revolta dos componentes I
Exercícios que foram atendidos 3.

3 - Deve ser criado para a CEO um componente lightning que permita identificar quais clientes foram contatados ou não durante o processo de “Negociação”. (que não precisa realizar)

obs:*Caso não tenha esse status utilize algo próximo*

