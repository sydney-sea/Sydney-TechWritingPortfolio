# Being Independent vs Teaming with Stakeholders
**Objective:**
Analyze a piece of documentation to identify which piece of information a technical writer can independently research and which require consultation with Subject Matter Experts (SMEs).

**Documentation:** [YouTube Data API Overview](https://developers.google.com/youtube/v3/getting-started#resources)


| Independent Research | SME Consultation |
|:----------- |:------| 
| Prerequisites such as requesting an API key and creating a project in the developer’s console are standard across Google, and documentation exists that could be referenced for research. | YouTube-Specific resources would require SME consultation to ensure that the descriptions of resource types, such as ‘channel’, ‘video’, etc., are accurate, up-to-date, and reflect the intended usage.   |
| An introduction to JSON concepts and formatting can be found on their website, json.org.   | Additionally, YouTube-specific operations are supported for different types of resources. Consultation is needed to understand which resources are supported by which operations and ensure the chart is accurate and clear.    |
| Operations are a standard HTTP method that could be independently researched. Operations allow clients to interact with servers to retrieve, create, update, and delete resources.   | There is a quota for all API requests, which differs across operations. The limit changes across Google products and is calculated differently for each operation. SME expertise is needed to confirm the specific amount for YouTube and the cost for each operation.    |
