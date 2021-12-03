---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4ec9a4db669bf6a01e97176d66c36a414320dd84
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61295931"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
eventId := "event-id"
extensionId := "extension-id"
result, err := graphClient.GroupsById(&groupId).EventsById(&eventId).ExtensionsById(&extensionId).Get(nil)


```