---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bd0c3cad90b1017907d0790481b8bfafa33a0782
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098852"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
eventId := "event-id"
extensionId := "extension-id"
result, err := graphClient.GroupsById(&groupId).EventsById(&eventId).ExtensionsById(&extensionId).Get(options)


```