---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b739ee5ff818316054d58624721db9c48e54757a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098504"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTenantAppManagementPolicy()
isEnabled := true
requestBody.SetIsEnabled(&isEnabled)
applicationRestrictions := msgraphsdk.NewAppManagementConfiguration()
requestBody.SetApplicationRestrictions(applicationRestrictions)
applicationRestrictions.SetPasswordCredentials( []PasswordCredentialConfiguration {
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "passwordAddition",
        "maxLifetime": nil,
        "restrictForAppsCreatedAfterDateTime": "2021-04-01T10:37:00Z",
    }
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "passwordLifetime",
        "maxLifetime": "P4DT12H30M5S",
        "restrictForAppsCreatedAfterDateTime": "2019-01-01T10:37:00Z",
    }
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "symmetricKeyAddition",
        "maxLifetime": nil,
        "restrictForAppsCreatedAfterDateTime": "2021-04-01T10:37:00Z",
    }
    msgraphsdk.NewPasswordCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "symmetricKeyLifetime",
        "maxLifetime": "P40D",
        "restrictForAppsCreatedAfterDateTime": "2015-04-01T10:37:00Z",
    }
}
applicationRestrictions.SetKeyCredentials( []KeyCredentialConfiguration {
    msgraphsdk.NewKeyCredentialConfiguration(),
    SetAdditionalData(map[string]interface{}{
        "restrictionType": "asymmetricKeyLifetime",
        "maxLifetime": "P30D",
        "restrictForAppsCreatedAfterDateTime": "2015-01-01T10:37:00Z",
    }
}
options := &msgraphsdk.DefaultAppManagementPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Policies().DefaultAppManagementPolicy().Patch(options)


```