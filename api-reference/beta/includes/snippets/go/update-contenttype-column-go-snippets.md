---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5594304e6b032610467d427ba579b2632bb0ce9c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340353"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewColumnDefinition()
required := true
requestBody.SetRequired(&required)
hidden := false
requestBody.SetHidden(&hidden)
propagateChanges := false
requestBody.SetPropagateChanges(&propagateChanges)
siteId := "site-id"
contentTypeId := "contentType-id"
columnDefinitionId := "columnDefinition-id"
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).ColumnsById(&columnDefinitionId).Patch(requestBody)


```