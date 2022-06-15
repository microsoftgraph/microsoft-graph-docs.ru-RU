---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 260728cc77cfb33ed8688009ec3fa7393f316b51
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66099545"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProfileCardProperty()
requestBody.SetAnnotations( []ProfileCardAnnotation {
    msgraphsdk.NewProfileCardAnnotation(),
    SetLocalizations( []DisplayNameLocalization {
        msgraphsdk.NewDisplayNameLocalization(),
languageTag := "no-NB"
        SetLanguageTag(&languageTag)
displayName := "Kostnads Senter"
        SetDisplayName(&displayName)
    }
}
organizationId := "organization-id"
profileCardPropertyId := "profileCardProperty-id"
graphClient.OrganizationById(&organizationId).Settings().ProfileCardPropertiesById(&profileCardPropertyId).Patch(requestBody)


```