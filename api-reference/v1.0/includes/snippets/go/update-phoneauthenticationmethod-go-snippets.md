---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewPhoneAuthenticationMethod()
phoneNumber := "+1 2065555554"
requestBody.SetPhoneNumber(&phoneNumber) 
phoneType := graphmodels.MOBILE_AUTHENTICATIONPHONETYPE 
requestBody.SetPhoneType(&phoneType) 

graphClient.Me().Authentication().PhoneMethodsById("phoneAuthenticationMethod-id").Patch(context.Background(), requestBody, nil)


```