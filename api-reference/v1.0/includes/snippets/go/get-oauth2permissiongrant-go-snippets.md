---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1125d1a948d51cd3fb969b30b89d75bdd7aaa436
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342942"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

oAuth2PermissionGrantId := "oAuth2PermissionGrant-id"
result, err := graphClient.Oauth2PermissionGrantsById(&oAuth2PermissionGrantId).Get()


```