---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f777c8ff12ef77dc3231aeb43a37eeb8cdcc5b6e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088767"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedRoleAssignmentRequestId := "privilegedRoleAssignmentRequest-id"
result, err := graphClient.PrivilegedRoleAssignmentRequestsById(&privilegedRoleAssignmentRequestId).Cancel().Post(options)


```