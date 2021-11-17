---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c949de9bb7f93ff81f18bcc1b25b9917e049f70f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030877"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewGroupLifecyclePolicy()
groupLifetimeInDays := int32(180)
requestBody.SetGroupLifetimeInDays(&groupLifetimeInDays)
managedGroupTypes := "Selected"
requestBody.SetManagedGroupTypes(&managedGroupTypes)
alternateNotificationEmails := "admin@contoso.com"
requestBody.SetAlternateNotificationEmails(&alternateNotificationEmails)
options := &msgraphsdk.GroupLifecyclePolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
groupLifecyclePolicyId := "groupLifecyclePolicy-id"
graphClient.GroupLifecyclePoliciesById(&groupLifecyclePolicyId).Patch(options)


```