### Full Stack Development in ServiceNow

- Database
- servers
- systems engineering
- clients
- opcionais
  - mobile stack
  - web stack
  - native application
    ![[img1.png]]Graphic comparing the Development Technology Stack to the ServiceNow Technology Stack:
    UX/UI : UX/UI; 
    Front End (Angular, React, Vue) : Experience (Workspace, Mobile, Portal);
    Back End (Java, .Net, API, Bus Logic) : Security (ACLs) , Logic & Automation (Business Rules, Script Includes, Flow); 
    Database. (MonoDB, MySQL, App server) : Data (Tables, Integration Spokes)

---

### Now Plataform Development Tools

- **Tools** :
  - **Studio:** Closer in usability to traditional integrated development environments (IDE). 
    - View files that comprise their application in the Application Explorer.
    - Add new files to their application using a single Create Application File interface.
    - Navigate to files using familiar search-by-name or by-type behavior with the Go to dialog.
    - Find code both within and outside an application using the Code Search tool.
    - Operate on multiple files at once using the tabbed interface.
    - Operate on multiple applications at once using multiple studio windows.
    - Publish the application to company instances or the ServiceNow Store.
    - View information about the current application from the Status Bar.
      ![[img2.png]]
  - **App Engine Studio:** A low-code visual app development environment to rapidly stand up applications and make quick adjustments.
    - Data = datebase (entidades)
    - Experience = Front end (UI/UX)
    - Logic and automation = Back end (regras de negócios)
    - Security = Back end 2 (Roles e permissões)
    - Tools:
      - UI Builder
        - Create and edit custom portal and workspace UI experiences using a highly configurable UI development tool.
      - Table Builder
        - schema view, spreadsheet view, flows, and PDF extractor are available in Table Builder.
      - Catalog Builder
        - Create and edit a catalog item using a guided tool
      - Flow Designer
        - Create and edit flows
      - Mobile App Builder
        - The Mobile App Builder is a development tool used to create and manage screens and records within ServiceNow mobile applications.

---

### App development Lifecycle in AES

- Develop at the development instance
- tested in the homolog instance
  - if found error, fixed at development instance
- when ready, published at the production instance
  ![[img3.png]]

---
## Build an Application
- **Components**
	- Data
	- Experience
	- Logic and automation
	- Security
- Recomendação: pensar em solução end-end --Jornadas
- Dentro do app engine as aplicações seguem o padrão de conteinerização

---

## Data and Security layer
### Table Creation and Data Options

- Temos 3 principais maneiras de iniciar os dados dentro do app engine
	- Importando uma Spreadsheet (.xlsx)
	- Criando uma tabela em branco e configurando-a
	- Criando uma integração de dados (config, execution and schedule imports from .xlsx)

- Applications can use multiple types of tables such as:
	-  **Base tables:** contain the primary application records
	-  **Reference** **tables:** are used for lookups
	When you create your table in ServiceNow, existing ServiceNow tables can provide the allowable reference lookup values for your fields.![[img4.png]]
	