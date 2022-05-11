---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 23c5e2a26b4f8a07d71251632e3e7c5c1c2a36ed
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340108"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewStore()
defaultLanguageTag := "en-US"
requestBody.SetDefaultLanguageTag(&defaultLanguageTag)
graphClient.TermStore().Patch(requestBody)


```