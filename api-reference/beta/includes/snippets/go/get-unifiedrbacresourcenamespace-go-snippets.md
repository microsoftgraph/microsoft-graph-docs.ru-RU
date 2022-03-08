---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1f22fdc157800944bf3dfec3218163b3e3158a21
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339825"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRbacResourceNamespaceId := "unifiedRbacResourceNamespace-id"
result, err := graphClient.RoleManagement().Directory().ResourceNamespacesById(&unifiedRbacResourceNamespaceId).Get(nil)


```