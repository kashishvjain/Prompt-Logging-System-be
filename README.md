<p align="center">
  <img src="https://cdn4.iconfinder.com/data/icons/bold-blue-symbols-vol-2/1024/move_in_go_proceed_prompt_app_mobile-512.png" width="100" alt="project-logo">
</p>
<p align="center">
    <h1 align="center">PROMPT-LOGGING-SYSTEM-BE</h1>
</p>
<p align="center">
    <em>Empowering seamless API interactions, unleash innovation.</em>
</p>
<p align="center">
	<img src="https://img.shields.io/github/last-commit/kashishvjain/Prompt-Logging-System-be?style=default&logo=git&logoColor=white&color=0080ff" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/kashishvjain/Prompt-Logging-System-be?style=default&color=0080ff" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/kashishvjain/Prompt-Logging-System-be?style=default&color=0080ff" alt="repo-language-count">
<p>
<p align="center">
	<!-- default option, no dependency badges. -->
</p>

<br><!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary><br>

- [ Overview](#-overview)
- [ Features](#-features)
- [ Repository Structure](#-repository-structure)
- [ Modules](#-modules)
- [ Getting Started](#-getting-started)
  - [ Installation](#-installation)
  - [ Usage](#-usage)
  - [ Tests](#-tests)
- [ Project Roadmap](#-project-roadmap)
- [ Contributing](#-contributing)
- [ License](#-license)
- [ Acknowledgments](#-acknowledgments)
</details>
<hr>

##  Overview

The Prompt-Logging-System-be project is a NestJS API logging system that manages business logic, API endpoints, and HTTP exception handling. It integrates services such as ClickHouse for data storage, OpenAI for chat completion, and validation tools for input integrity. This project facilitates seamless interaction between components within a robust architecture, enabling developers to store and query data efficiently while ensuring system reliability and data security.

---

##  Features

|    |   Feature          | Description |
|----|--------------------|---------------------------------------------------------------|
| ⚙️  | **Architecture**   | NestJS framework used with modular structure and Decorators for abstraction. |
| 🔩 | **Code Quality**   | Linting with ESLint, testing with Jest, and strong TypeScript usage. |
| 📄 | **Documentation**  | Moderate documentation covering config, modules, and API endpoints. |
| 🔌 | **Integrations**   | Integrates Axios, OpenAI SDK, ClickHouse client for data handling. |
| 🧩 | **Modularity**     | Codebase structured into modules for reusability and maintainability. |
| 🧪 | **Testing**        | Jest for unit testing, End-to-End testing with Supertest. |
| ⚡️  | **Performance**    | Efficient data handling with ClickHouse, async methods improve speed. |
| 🛡️ | **Security**       | Configurable validation pipe for input data, handled bad requests. |
| 📦 | **Dependencies**   | Key libs: NestJS, Axios, ClickHouse, OpenAI SDK, Jest, ESLint. |

---

##  Repository Structure

```sh
└── Prompt-Logging-System-be/
    ├── README.md
    ├── dist
    │   ├── app.controller.d.ts
    │   ├── app.controller.js
    │   ├── app.controller.js.map
    │   ├── app.module.d.ts
    │   ├── app.module.js
    │   ├── app.module.js.map
    │   ├── app.service.d.ts
    │   ├── app.service.js
    │   ├── app.service.js.map
    │   ├── http-exception.filter.d.ts
    │   ├── http-exception.filter.js
    │   ├── http-exception.filter.js.map
    │   ├── main.d.ts
    │   ├── main.js
    │   ├── main.js.map
    │   ├── proxy-api
    │   └── tsconfig.build.tsbuildinfo
    ├── nest-cli.json
    ├── package-lock.json
    ├── package.json
    ├── src
    │   ├── app.controller.spec.ts
    │   ├── app.controller.ts
    │   ├── app.module.ts
    │   ├── app.service.ts
    │   ├── http-exception.filter.ts
    │   ├── main.ts
    │   └── proxy-api
    ├── test
    │   ├── app.e2e-spec.ts
    │   └── jest-e2e.json
    ├── tsconfig.build.json
    └── tsconfig.json
```

---

##  Modules

<details closed><summary>.</summary>

| File                                                                                                            | Summary                                                                                                                                                                                                                                                                                                                                                                                         |
| ---                                                                                                             | ---                                                                                                                                                                                                                                                                                                                                                                                             |
| [package.json](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/package.json)               | Implements key npm scripts for building, testing, and starting the NestJS API. Dependencies include @nestjs packages, Axios, ClickHouse client, OpenAI SDK, and Date-fns. Dev dependencies cover testing with Jest and linting with ESLint.                                                                                                                                                     |
| [package-lock.json](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/package-lock.json)     | The code file `app.service.js` in the `Prompt-Logging-System-be` repository serves a critical role in handling and managing the applications business logic. It provides essential services and functionality to support the systems core operations. Its main purpose is to encapsulate key business logic, enabling seamless interaction between different components within the application. |
| [tsconfig.json](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/tsconfig.json)             | Defines TypeScript compiler options to enable ES2021 features and generate CommonJS modules. Maintains source maps, metadata, and synthetic imports for the NestJS logging system. Implements decorators for abstraction with experimental decorators support.                                                                                                                                  |
| [nest-cli.json](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/nest-cli.json)             | Enables Nest.js schematics in the project. Specifies source root and compiler options for the @nestjs/schematics collection. Facilitates configuring project settings for efficient development and build processes.                                                                                                                                                                            |
| [tsconfig.build.json](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/tsconfig.build.json) | Defines build configuration, inheriting settings, and excluding unnecessary folders and test files. Facilitates TypeScript compilation for production, optimizing build output.                                                                                                                                                                                                                 |

</details>

<details closed><summary>test</summary>

| File                                                                                                         | Summary                                                                                                                                                                           |
| ---                                                                                                          | ---                                                                                                                                                                               |
| [jest-e2e.json](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/test/jest-e2e.json)     | Configures Jest for end-to-end tests in the project. Sets up module extensions, test environment, regex patterns, and transformation rules to enable testing of TypeScript files. |
| [app.e2e-spec.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/test/app.e2e-spec.ts) | Tests the API endpoints by creating a NestJS testing module with the AppModule, initializing the application, and sending a GET request to check the response status and content. |

</details>

<details closed><summary>src</summary>

| File                                                                                                                          | Summary                                                                                                                                                                                                                                    |
| ---                                                                                                                           | ---                                                                                                                                                                                                                                        |
| [http-exception.filter.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/http-exception.filter.ts) | Implements HTTP exception handling for the NestJS app. Captures and processes HTTP exceptions, extracting status codes and messages to be sent as JSON responses.                                                                          |
| [app.module.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/app.module.ts)                       | Defines core app structure, linking controllers and services. Utilizes ValidationPipe for input validation and HttpExceptionFilter for error handling. Integrates ProxyApiModule for extended functionality within the Nest.js server.     |
| [app.controller.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/app.controller.ts)               | Defines AppController with a single method to fetch a greeting from AppService. This file orchestrates service interactions within the NestJS API architecture.                                                                            |
| [app.controller.spec.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/app.controller.spec.ts)     | Verifies AppController functionality to return Hello World! in the NestJS project.                                                                                                                                                         |
| [app.service.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/app.service.ts)                     | Implements a service for the NestJS framework that retrieves a simple greeting message.                                                                                                                                                    |
| [main.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/main.ts)                                   | Implements the main function to initialize a NestJS application, setting up global exception filtering and defining the port for the application to listen on, as part of the larger logging system architecture in the parent repository. |

</details>

<details closed><summary>src.proxy-api</summary>

| File                                                                                                                                            | Summary                                                                                                                                                                                                                                                              |
| ---                                                                                                                                             | ---                                                                                                                                                                                                                                                                  |
| [clickhouse.service.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/clickhouse.service.ts)               | Handles storing and querying data in ClickHouse dataset. Provides methods to insert responses and query data based on filters and time period. Additionally, calculates total input and output tokens from the queried data.                                         |
| [proxy-api.module.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/proxy-api.module.ts)                   | Defines a module for proxy API services including ProxyApiController, ProxyApiService, OpenAIService, ClickHouseService, and ResponseApiService. Manages controllers and providers for seamless integration within the NestJS architecture of the parent repository. |
| [proxy-api.service.spec.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/proxy-api.service.spec.ts)       | Verifies the definition of the ProxyApiService by creating a testing module and checking if the service is defined. Contributes to ensuring the functionality and correctness of the proxy API service in the project architecture.                                  |
| [openaiService.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/openaiService.ts)                         | Implements OpenAI API integration for chat completion using custom headers in parent repositorys proxy-api module. Fetches response from OpenAI and logs it.                                                                                                         |
| [proxy-api.controller.spec.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/proxy-api.controller.spec.ts) | Verifies ProxyApiController definition. Sets up test module with ProxyApiController and ProxyApiService, ensuring controller is defined.                                                                                                                             |
| [responseAPIUtils.service.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/responseAPIUtils.service.ts)   | Defines ResponseAPI structure and operations for creating, updating successful and failed responses in the Prompt Logging System. Manages request details and token counts to generate response data.                                                                |
| [proxy-api.service.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/proxy-api.service.ts)                 | Creates a service to interact with external APIs, store responses in a ClickHouse dataset, and query the dataset with filters. Calculates total input and output tokens from the dataset for metrics reporting.                                                      |
| [proxy-api.controller.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/proxy-api.controller.ts)           | Defines API endpoints for a proxy service to create, retrieve, and get metrics using NestJS controllers. Validates input data with a configurable validation pipe. Handles bad requests with a defined HTTP exception.                                               |

</details>

<details closed><summary>src.proxy-api.dto</summary>

| File                                                                                                                                      | Summary                                                                                                                                                                                                                                                                        |
| ---                                                                                                                                       | ---                                                                                                                                                                                                                                                                            |
| [create-proxy-api.dto.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/dto/create-proxy-api.dto.ts) | Defines MetadataDto and CreateProxyApiDto classes with validation rules for user input, central to data integrity in the proxy API functionality.                                                                                                                              |
| [update-proxy-api.dto.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/dto/update-proxy-api.dto.ts) | Defines DTO for updating a proxy API by extending the create DTO with partial properties, enabling API updates with only specified fields.                                                                                                                                     |
| [QueryParams.dto.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/dto/QueryParams.dto.ts)           | Defines classes for filtering data through query parameters in the parent repository. `FiltersDto` specifies filter options like model, status, and environment. `QueryParamsDto` utilizes `FiltersDto` as a nested object to enable data filtering based on query parameters. |

</details>

<details closed><summary>src.proxy-api.entities</summary>

| File                                                                                                                                   | Summary                                                                                                                                                      |
| ---                                                                                                                                    | ---                                                                                                                                                          |
| [proxy-api.entity.ts](https://github.com/kashishvjain/Prompt-Logging-System-be/blob/master/src/proxy-api/entities/proxy-api.entity.ts) | Defines Proxy API entity model for the logging system. It aims to encapsulate data attributes and behavior related to proxy APIs in the system architecture. |

</details>

---

##  Getting Started

**System Requirements:**

* **TypeScript**

###  Installation

<h4>From <code>source</code></h4>

> 1. Clone the Prompt-Logging-System-be repository:
>
> ```console
> $ git clone https://github.com/kashishvjain/Prompt-Logging-System-be
> ```
>
> 2. Change to the project directory:
> ```console
> $ cd Prompt-Logging-System-be
> ```
>
> 3. Install the dependencies:
> ```console
> $ npm install
> ```

###  Usage

<h4>From <code>source</code></h4>

> Run Prompt-Logging-System-be using the command below:
> ```console
> $ npm run build && node dist/main.js
> ```

###  Tests

> Run the test suite using the command below:
> ```console
> $ npm test
> ```

---

