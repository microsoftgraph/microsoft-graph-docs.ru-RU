---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 34b37dd29cdad124ab9666bb0d5610b2f93abd11
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314375"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedRoleAssignmentRequestId := "privilegedRoleAssignmentRequest-id"
result, err := graphClient.PrivilegedRoleAssignmentRequestsById(&privilegedRoleAssignmentRequestId).Cancel(privilegedRoleAssignmentRequest-id).Post()


```