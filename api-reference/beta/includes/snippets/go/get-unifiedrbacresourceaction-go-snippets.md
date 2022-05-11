---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6690b7c2bf18b4a7a1d42c6e9ef3dc0ed0a1c381
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340923"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

unifiedRbacResourceNamespaceId := "unifiedRbacResourceNamespace-id"
unifiedRbacResourceActionId := "unifiedRbacResourceAction-id"
result, err := graphClient.RoleManagement().Directory().ResourceNamespacesById(&unifiedRbacResourceNamespaceId).ResourceActionsById(&unifiedRbacResourceActionId).Get()


```