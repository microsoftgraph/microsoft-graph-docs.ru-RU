---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2efdad35a9f360f02e12be01631ec862306a26e3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342904"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
userScopeTeamsAppInstallationId := "userScopeTeamsAppInstallation-id"
graphClient.UsersById(&userId).Teamwork().InstalledAppsById(&userScopeTeamsAppInstallationId).Delete()


```