---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4cd248d9ea68b7c0c8bf9f6e0857a85fd26ee6a6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65342284"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
appRoleAssignmentId := "appRoleAssignment-id"
graphClient.UsersById(&userId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete()


```