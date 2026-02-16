# Architecture Overview

## Sequence Diagram

```plaintext
User -> API Gateway -> Auth Service -> Auth Database

Auth Database -- Success --> Data Service -> App Database

Auth Database -- Failure --> API Gateway
```  

This architecture includes proper authentication validation and conditional response paths.