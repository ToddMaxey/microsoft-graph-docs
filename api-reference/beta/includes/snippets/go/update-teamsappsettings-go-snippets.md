---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewTeamsAppSettings()
isChatResourceSpecificConsentEnabled := true
requestBody.SetIsChatResourceSpecificConsentEnabled(&isChatResourceSpecificConsentEnabled) 

graphClient.Teamwork().TeamsAppSettings().Patch(context.Background(), requestBody, nil)


```