---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7e7463fad1f90ae26b1d79bd6b7fbb0213ea9996
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996012"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSecureScoreControlProfile()
vendorInformation := msgraphsdk.NewSecurityVendorInformation()
requestBody.SetVendorInformation(vendorInformation)
provider := "SecureScore"
vendorInformation.SetProvider(&provider)
vendorInformation.SetProviderVersion(nil)
vendorInformation.SetSubProvider(nil)
vendor := "Microsoft"
vendorInformation.SetVendor(&vendor)
requestBody.SetAdditionalData(map[string]interface{}{
    "assignedTo": "",
    "comment": "control is reviewed",
    "state": "Reviewed",
}
options := &msgraphsdk.SecureScoreControlProfileRequestBuilderPatchOptions{
    Body: requestBody,
}
secureScoreControlProfileId := "secureScoreControlProfile-id"
graphClient.Security().SecureScoreControlProfilesById(&secureScoreControlProfileId).Patch(options)


```