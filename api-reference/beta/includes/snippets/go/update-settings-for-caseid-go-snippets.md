---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewCaseSettings()
redundancyDetection := graphmodels.NewRedundancyDetectionSettings()
isEnabled := false
redundancyDetection.SetIsEnabled(&isEnabled) 
similarityThreshold := int32(70)
redundancyDetection.SetSimilarityThreshold(&similarityThreshold) 
minWords := int32(12)
redundancyDetection.SetMinWords(&minWords) 
maxWords := int32(400000)
redundancyDetection.SetMaxWords(&maxWords) 
requestBody.SetRedundancyDetection(redundancyDetection)
topicModeling := graphmodels.NewTopicModelingSettings()
isEnabled := false
topicModeling.SetIsEnabled(&isEnabled) 
ignoreNumbers := false
topicModeling.SetIgnoreNumbers(&ignoreNumbers) 
topicCount := int32(50)
topicModeling.SetTopicCount(&topicCount) 
dynamicallyAdjustTopicCount := false
topicModeling.SetDynamicallyAdjustTopicCount(&dynamicallyAdjustTopicCount) 
requestBody.SetTopicModeling(topicModeling)
ocr := graphmodels.NewOcrSettings()
isEnabled := true
ocr.SetIsEnabled(&isEnabled) 
maxImageSize := int32(12000)
ocr.SetMaxImageSize(&maxImageSize) 
requestBody.SetOcr(ocr)

graphClient.Compliance().Ediscovery().CasesById("case-id").Settings().Patch(context.Background(), requestBody, nil)


```