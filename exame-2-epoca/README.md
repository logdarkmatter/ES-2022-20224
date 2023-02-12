**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**

# Software Engineering - Exame de 2º Época

# Use Case - ULHT CONDO MANAGER:
Pretende-se desenvolver um Software com o objetivo de efetuar a gestão de condomínios para uma empresa (Condos Managers ULHT) com o objetivo de gerir as necessidades da sua carteira de clientes. Este Software deve seguir a seguinte arquitetura: um single back-end desenvolvido em Java com ligação a uma base de dados MySQL através de um ORM; uma aplicação web desenvolvida em Angular e uma aplicação hibrida para Android e IOS. Ambos comunicam com o back-end através de serviços REST.

* **O Software deve garantir os requisitos funcionais abaixo enumerados:**
* Criação de Condomínios;
    * Podem ser criados condomínios em número ilimitado;
* Criação da ficha de condómino;
    * Devem ser identificadas as frações que pertencem a cada condómino;
    * Valor do condomínio em questão é igual para todos os condóminos independentemente da tipologia da fração;
    * Devem ser validados e persistidos os seguintes documentos:
        * 1 - CC ou Bilhete de Identidade – (Data válida e Número de identificação válido);
        * 1 - Certidão de compra da fração (PDF ou Docx);
    * Deve ser possível fazer a configuração de contas bancárias dos condóminos para opagamento do respetivo condomínio.
* Cada condomínio deve ter a sua conta corrente (Saldo acumulado disponível);
* Deve ser possível a configuração de um sistema de penalidades:
    * Se o condómino estiver em dívida com o pagamento condomínio é penalizado e o valor em falta é acrescido ao mês seguinte com uma taxa de juro de 1.5%.
* Funcionalidade de criação de orçamentos:
    * Podem existir mais do que um orçamento no mesmo período temporal mas para finalidades diferentes. Os orçamentos devem cumprir as seguintes regras:
    * O orçamento inicial e a sua finalidade só pode ser criado pelo gestor de condomínio;
    * Os orçamentos criados pelo gestor de condomínio têm de ser aprovados pelos restantes condóminos pertencentes ao condomínio em questão:
        * Se o condómino estiver em incumprimento deixa de exercer funções de aprovação. (É ignorado pela regra anterior). (Exceção)
    * Se o valor do orçamento ultrapassar o saldo disponível na conta corrente o orçamento não pode ser aprovado;
    * O orçamento tem de ser aprovado até à data limite que foi estipulada, caso contrário é cancelado automaticamente.
* Os documentos carregados ssão e guardados em Blobs na BD.

# Exercise - Part 1 (Requirements Gathering with User Stories)

**Let's start** 🏁:
1. Go to Trello and create a board with the name of your solution/product;
    * Share the board with all the professors (p5617@ulusofona.pt - Pedro Perdigão & p5932@ulusofona.pt - Rui Santos);
    * Create a "To do" column and create a new card with:
        * Our full-name;
        * Student number;

2. Read the use case above regarding the "ULHT Condo Manager". You must **must identify** the following items:
    * 1 epics;
    * 3 features for the related epic;
    * 5 user stories for each feature;
    * 2 technical user stories for each epic.

3. Before you start brainstorming the user stories, write down on a new Trello card one a sentence that briefly characterising the purpose/value of your system.

4. Add the estimation value to the User Story Trello card - You can add the estimation value directly on the title or in the description of the card;
    * Evaluate our estimations and take conclusions.

**Notes**:
* Make sure	that the 10	user stories fulfill the **INVEST**	criteria;
* Remember to keep them in the correct format: “As a ____, I need a ____ in order to ____”.

# Exercise - Part 2 (Scrum/Kanban Board workflow, User Stories prioritization & Group U/S into Sprints)

**Let's start** 🏁:
1. Picture which states do you think it makes sense, while you are developing a feature, to be present visibly in the board columns and create those columns;
   * Ensure you predict undesired scenarios;
   * Comparing to a state machine can be helpful;
   * Ensure critical Scrum components are contemplated in this board;
   * Make usage of **labels** in Trello, they will be helpful for some organization 🤓
2. Take a look at the User Stories you created in Part 1 and define priorities, which stories should be done first, last and in between;
   * One way of doing this is to group US subjects as a whole and see from a higher level respective;
3. Now that you have the US grouped, it's time to ensemble the course of action through the weeks/months;
   * Think of Sprints as 2 weeks of work;
   * Remember when we talked about **labels**? 😉 Now it's a good time to put in practice;
   * Organize the cards in the board to be visible which are going to be done in the first Sprint. Assume you will start the first sprint in the time you are doing this laboratory;
4. Review the whole process until now and picture in the long term to see it gathers all requirements.


# Exercise - 3 (Write Acceptance criteria (AC) for User Stories done in Part 2)

**Let's start** 🏁:
1. Brainstorm the following:
    * on the most valuable top 10 user stories (To do U/S & the top on the product backlog (User Story column)) at least:
        * 1-N Acceptance criteria (AC) in GWT-scenario-oriented format.

# Exercise - 4 (Entity-Relationship Diagram Symbols and Notation)

1. Create a new column in your Trello board named "UML" and a new Trello card inside the new column named "Conceptual ERD";
2. Look in to our user stories, acceptance criteria and future of the solution (big picture) and using the tool [Diagrams.net aka Draw.io](https://app.diagrams.net/) please elaborate the Conceptual ERD for your solution:
    * **Identify the entities:** The first step in making an ERD is to identify **ALL** the entities you will use. An entity is nothing more than a rectangle with a description of something that your system stores information about. This could be a customer, a manager, an invoice, a schedule, etc. Draw a rectangle for each entity you can think of on your page. Keep them spaced out a bit;
    * **Identify relationships:** Look at your entities, are they related? If so draw a solid line connecting the two entities and add a diamond between them with a brief description of how they are related;
    * **Add attributes:** Any key attributes of entities should be added using oval-shaped symbols;
    * **Complete the diagram:** Continue to connect the entities with lines, and adding diamonds to describe each relationship until all relationships have been described. Each of your entities may not have any relationships, some may have multiple relationships.
3. After concluding your Conceptual ERD, export it as a PNG and import the image into our new card "Conceptual ERD";

# Exercise - 5 (UML - Class Diagram)

**Let's start** 🏁:
1. In your Trello board in the column "UML" create a new Trello card column named "Class Diagram";
2. Look into your Conceptual Diagram done in [Laboratory 4](https://github.com/logdarkmatter/ES-2022-2023/tree/main/lab4) and map yoor Conceptual Diagram into a new Class Diagram. Please make sure that you add access modifiers, types and enumerators to your attributes; also make sure you have the 3 mandatory sections in the diagram (upper, middle and bottom);
    * Please make sure you use as much a Domain-Driven Design approach where you can personify your classes and add operation to it.  
3. After concluding your Conceptual ERD, export it as a PNG and import the image into our new card "Class Diagram";

**Tools**
* You can use:
    * [Diagrams.net aka Draw.io](https://app.diagrams.net/);
    * [Visual Paradigm](https://www.visual-paradigm.com/download/community.jsp).


# Exercise - 6 (UI/UX - Wireframes)

**Let's start** 🏁:
1. In your Trello board create a new column anmed "UI/UX";
2. In your Trello board in the new column "UI/UX" create a new Trello card column named "Wireframes";
3. Now you must design wireframes that represent the 3 features that you have created for your solution - Check you feature cards on the trello board;
    * The wireframes forms and attributes must match your logical and conceptual diagram attributes;
4. After concluding your wireframes, export them as a PNG and import the image into our new card "Wireframes".

**Tools**
* Some suggestions you can use:
    * [Diagrams.net aka Draw.io](https://app.diagrams.net/);
    * [https://balsamiq.com/](https://balsamiq.com/);
        * For the product key check the course main page [here](https://moodle.ensinolusofona.pt/course/view.php?id=7927#section-0);
    * [Figma](https://www.figma.com/);
    * [Miro](https://miro.com/pt/);
    * Powerpoint;
    * etc.

# Exercise - 7 (UI/UX - Wireframes)

**Let's start** 🏁:
1. In your Trello board in the previously created column "UML" create a new Trello card column named "Sequence Diagrams";
2. Now you must design **3 method logic diagrams** that represent a specific CRUD operation in or system;
    * CRUD examples:
        * Search data like Clients, Reservations, trips, etc;
        * Save or Upadate data like clients, reservations, trips etc;
        * Delete data like client, reservations, trips, etc. 
3. Please ensure that in our 3 diagrams you have enough Lifelines (e.g: 4); Self Messages to represent functions in certain object, and fragments like alt or loop.
4. After concluding your diagrams, export them as a PNG and import the image into our new card "Sequence Diagrams".

**Tools**
* Some suggestions you can use:
    * [Visual Paradigm](https://www.visual-paradigm.com/download/community.jsp).

# Good Luck!! 🍀 
