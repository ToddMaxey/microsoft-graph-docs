---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new TokenLifetimePolicy();
$requestBody->setDefinition(['definition-value', ]);

$requestBody->setDisplayName('displayName-value');

$requestBody->setIsOrganizationDefault(true);



$graphServiceClient->policies()->tokenLifetimePoliciesById('tokenLifetimePolicy-id')->patch($requestBody);


```