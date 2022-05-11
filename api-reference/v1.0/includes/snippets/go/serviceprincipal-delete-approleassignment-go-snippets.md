---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 58dbd91e9673335fef7c4c430030ad2fd24f0317
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343304"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

servicePrincipalId := "servicePrincipal-id"
appRoleAssignmentId := "appRoleAssignment-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).AppRoleAssignmentsById(&appRoleAssignmentId).Delete()


```