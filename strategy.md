[Refactory guru - Strategy](https://refactoring.guru/pt-br/design-patterns/strategy/)

Resumo:

Proposito: Permite definir uma família de algoritmos de modo que sejam intercambiáveis em tempo de execucao.
Problema: Classe que faz algo específico em diversas maneiras(algoritmos) diferente.
Solucao: Extrair todos esses algoritmos/maneiras para classes separadas.


Anotacoes:

A classe original que precisa ser refatorada 'e chamada contexto.
O contexto delega o trabalho para um objeto estratégia ao invés de executá-lo por conta própria.
O contexto não é responsável por selecionar um algoritmo apropriado para o trabalho.
O cliente passa o algoritmo apropriado para o contexto.
O contexto tem um método para trocar a estratégia.
O cliente(ex: botões na interface de usuário), podem substituir o comportamento/estrategia selecionado por um outro.
O Cliente cria um objeto estratégia específico e passa ele para o contexto. O contexto expõe um setter que permite o cliente mudar a estratégia associada com contexto durante a execução.

