---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewAccessPackageCatalog()
displayName := "Catalog One"
requestBody.SetDisplayName(&displayName) 

graphClient.IdentityGovernance().EntitlementManagement().CatalogsById("accessPackageCatalog-id").Patch(context.Background(), requestBody, nil)


```