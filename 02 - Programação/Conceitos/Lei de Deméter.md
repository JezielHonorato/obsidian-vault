A **Lei de Deméter** (Law of Demeter - LoD), também conhecida como "**Princípio do Mínimo Conhecimento**", é uma diretriz de design de software, especialmente aplicada em programação orientada a objetos, que busca reduzir o acoplamento entre as classes.

Em termos simples, ela pode ser resumida em: **"Um objeto deve conversar apenas com seus amigos mais próximos; não fale com estranhos."**

Isso significa que um método de um objeto (vamos chamá-lo de Objeto A) só deve invocar métodos ou acessar propriedades dos seguintes tipos de objetos:

1. **O próprio objeto A.**
2. **Objetos que foram passados como parâmetros para o método de A.**
3. **Objetos que foram criados/instanciados pelo método de A.**
4. **Objetos que são componentes diretos (atributos/propriedades) do Objeto A.**
5. (Em alguns contextos) **Variáveis globais acessíveis ao Objeto A.**

**O que a Lei de Deméter busca evitar?**

Ela visa evitar "cadeias de chamadas" em cascata, como `objetoA.getObjetoB().getObjetoC().getMetodoD()`. Essa prática viola a Lei de Deméter porque o `objetoA` está "conhecendo" e interagindo com detalhes internos de `objetoB` e `objetoC`, que são "estranhos" para ele. Se a estrutura interna de `objetoB` ou `objetoC` mudar, o `objetoA` precisará ser alterado, aumentando o acoplamento e diminuindo a manutenibilidade do código.

**Benefícios de seguir a Lei de Deméter:**

- **Redução do acoplamento:** As classes se tornam menos dependentes umas das outras, tornando o código mais modular e flexível a mudanças.
- **Melhora na manutenibilidade:** Alterações em uma parte do sistema têm menos probabilidade de quebrar outras partes, facilitando a manutenção e a evolução do software.
- **Aumento da reusabilidade:** Classes com baixo acoplamento são mais fáceis de serem reutilizadas em diferentes contextos.
- **Código mais legível e compreensível:** O fluxo de informações se torna mais claro, pois os objetos têm responsabilidades bem definidas e interagem apenas com seus "amigos" diretos.
- **Facilidade de teste:** Classes com baixo acoplamento são mais fáceis de serem testadas em isolamento, pois suas dependências são mínimas e podem ser facilmente "mockadas".
