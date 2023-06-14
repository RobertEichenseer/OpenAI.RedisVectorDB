# Redis Stack as Vector Database

## Content

### Example

An [end-to-end example](./src/Notebook/dotnet.ipynb) using .NET / C# to:

- Use Azure OpenAI to create embeddings / vector representation of information.
- Store the embeddings / vector representation in Redis as ```HashSet```
- Create a Redis Stack search index to semantically query the embeddings
- Query the embeddings using Redis Stack vector search functionality

### Environment creation

A [Azure CLI script](./src/CreateEnv/CreateEnv.azcli) to create all components to run the sample application. Including:

- Azure Resource Group
- Azure OpenAI Cognitive Service instance
- ```text-embedding-ada-002``` model deployment
- Redis Stack container executed on Azure Container Instance 