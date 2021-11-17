---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dda17d5ac9528ea302d92f189a39100960bd524b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61018171"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

permissionGrantPolicyId := "permissionGrantPolicy-id"
graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Delete(options)


```