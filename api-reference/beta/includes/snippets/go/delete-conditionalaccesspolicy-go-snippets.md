---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 30603d1d928f8e2a784f489e93b2c1ca003b843c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103239"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

conditionalAccessPolicyId := "conditionalAccessPolicy-id"
graphClient.Identity().ConditionalAccess().PoliciesById(&conditionalAccessPolicyId).Delete(options)


```