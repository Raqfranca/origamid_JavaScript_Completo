## JavaScript

### **Especificações**

JavaScript é uma linguagem leve, interpretada e baseada em objetos com funções de primeira classe.

**1. Linguagem leve**

Isso significa que o JavaScript foi projetado para ser simples e eficiente, sem exigir muitos recursos do sistema. Ele é otimizado para funcionar bem nos navegadores e em diferentes ambientes, tornando-o ideal para scripts curtos e rápidos.

    Exemplo de leveza: Você pode escrever um simples script para alterar o texto de um botão sem precisar carregar bibliotecas pesadas:

    document.querySelector('button').textContent = 'Clique aqui';

**2. Interpretada**

Linguagens interpretadas são aquelas que são executadas diretamente, sem a necessidade de uma etapa de compilação prévia (como ocorre em linguagens como C ou Java). O código JavaScript é interpretado e executado em tempo real pelo navegador ou ambiente de execução (como o Node.js).

**3. Baseada em objetos**

JavaScript é estruturada em torno de objetos, que são coleções de pares chave-valor e podem conter propriedades e métodos.

    Exemplo básico de objeto:

    const pessoa = {
      nome: 'João',
      idade: 25,
      falar: function () {
        console.log(`Olá, meu nome é ${this.nome}`);
      }
    };
    pessoa.falar(); // Saída: Olá, meu nome é João

Objetos são fundamentais em JavaScript, usados para representar dados e comportamentos de maneira organizada.

**4. Funções de primeira classe**

Isso significa que em JavaScript, funções são tratadas como cidadãos de primeira classe, ou seja:

    - Elas podem ser atribuídas a variáveis.

    - Podem ser passadas como argumentos para outras funções.

    - Podem ser retornadas por outras funções.

    Exemplo:

    // Função atribuída a uma variável
    const saudacao = function(nome) {
      return `Olá, ${nome}!`;
    };

    // Função passada como argumento
    function executar(funcao, nome) {
      console.log(funcao(nome));
    }

    executar(saudacao, 'Maria'); // Saída: Olá, Maria!

### **Aplicações**

**1. Desenvolvimento Web (Frontend)**

O JavaScript é a base para criar experiências interativas em páginas da web. Ele manipula o DOM, reage a eventos do usuário e permite a criação de interfaces dinâmicas.

Tecnologias associadas: React, Vue.js, Angular.

**2. Desenvolvimento Backend**

Com o Node.js, JavaScript pode ser usado no backend para criar servidores, APIs e sistemas completos.

Tecnologias associadas: Express.js, NestJS, Koa.js.

**3. Aplicações Mobile**

JavaScript permite criar aplicativos móveis com frameworks como React Native e Ionic, usando o mesmo código para Android e iOS.

**4. Aplicações Desktop**

Com Electron, você pode criar aplicativos desktop usando tecnologias web (HTML, CSS, JS).

**5. Automação de Tarefas**

JavaScript pode ser usado para automatizar tarefas repetitivas no desenvolvimento com ferramentas como Gulp e Webpack.

**6. Desenvolvimento de Jogos**

JavaScript é usado para criar jogos simples diretamente no navegador ou até jogos mais complexos com engines como Phaser.

**7. Integração com IoT**

JavaScript, com frameworks como Johnny-Five, permite programar dispositivos IoT, como robôs e sensores.

**8. Machine Learning**

Com bibliotecas como TensorFlow.js, é possível criar e treinar modelos de aprendizado de máquina diretamente no navegador ou no backend.

**9. APIs e Microserviços**

No backend, JavaScript é usado para criar APIs REST e sistemas baseados em microserviços.

**10. Automação de Testes**

JavaScript é amplamente usado para testes automatizados em aplicações web.

### **Servidor != API**

**O que é um servidor?**

Um servidor é um computador (físico ou virtual) ou software que processa e responde a solicitações feitas por outros dispositivos (chamados de clientes). Ele pode fornecer diversos serviços, como:

    - Hospedar sites e aplicações web.
    - Gerenciar bancos de dados.
    - Fornecer arquivos ou recursos para outros dispositivos.

**O que é uma API?**

Uma API (Interface de Programação de Aplicações) é um conjunto de regras que permite que dois sistemas se comuniquem. No contexto web, uma API geralmente fornece acesso a dados ou funcionalidades de um sistema para outros programas (ou sistemas) via rede.

API em ação:

    Um cliente (como um navegador ou aplicativo) faz uma requisição para a API.
    A API processa essa requisição e envia uma resposta (geralmente em formato JSON ou XML).

Exemplo:

Imagine que você tem um servidor que hospeda um site e uma API:

    Servidor: Gera e entrega páginas HTML para o navegador.
    API: Fornece dados dinâmicos (como uma lista de produtos ou informações do usuário) que são consumidos pelo frontend.
