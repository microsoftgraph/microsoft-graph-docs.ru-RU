---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2db0bb12bcb7ea17253b8b9bc7a3d9a788fe3b46
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341939"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
teamworkTagId := "teamworkTag-id"
graphClient.TeamsById(&teamId).TagsById(&teamworkTagId).Delete()


```