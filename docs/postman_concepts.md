## Postman concepts:

- Create Workspace
- Create Collection
- Create Environment
- Create Requests - GET/POST/UPDATE/DELETE (CRUD)

#### Variables:
- Scopes: global < collection < environment < data < local.

### Scripting:
- Postman has rich editor supporting javascript. It has 2 editors - Pre-request script & Test
- Execution order of scripts -  Pre-request script > Request > Response > Test

### Best Testing practices:
- Create Environment/Global/Collection variables to dynamically switch end points of APIs to test in different stages of QA Life cycle
- Use property transfer between requests
- Generate dynamic values when required into input payload
- Always have tests for each request. Verify if API responses returns expected status code with proper assertions
- Verify if Response Json Schema is displayed as expected
- Implement Try Catch Error Handling Mechanism for every automation test as Tear Down Script
- Use Request(s) chaining to chain multiple requests within test scripts
- For multiple data sets, run APIs by iterating the data from the CSV as a Data driven testing



