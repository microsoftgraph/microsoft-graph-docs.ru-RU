---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 78edc2d045560633a979ac41f9a24a8cff9ebe7c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088329"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRoleAssignmentScheduleRequestId := "unifiedRoleAssignmentScheduleRequest-id"
graphClient.RoleManagement().Directory().RoleAssignmentScheduleRequestsById(&unifiedRoleAssignmentScheduleRequestId).Cancel().Post(options)


```