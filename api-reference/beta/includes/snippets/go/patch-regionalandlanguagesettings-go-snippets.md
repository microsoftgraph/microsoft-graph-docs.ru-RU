---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7905172cfef2be869bb8620722cb39de537a250f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088521"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewRegionalAndLanguageSettings()
requestBody.SetAuthoringLanguages( []LocaleInfo {
    msgraphsdk.NewLocaleInfo(),
    SetAdditionalData(map[string]interface{}{
        "locale": "en-US",
    }
    msgraphsdk.NewLocaleInfo(),
    SetAdditionalData(map[string]interface{}{
        "locale": "es-MX",
    }
}
defaultRegionalFormat := msgraphsdk.NewLocaleInfo()
requestBody.SetDefaultRegionalFormat(defaultRegionalFormat)
locale := "en-US"
defaultRegionalFormat.SetLocale(&locale)
options := &msgraphsdk.RegionalAndLanguageSettingsRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Me().Settings().RegionalAndLanguageSettings().Patch(options)


```