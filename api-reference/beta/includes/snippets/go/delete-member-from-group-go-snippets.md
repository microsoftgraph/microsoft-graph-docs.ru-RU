---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e998ca244a0020ec997e04a9e17e72aa3d7350fc
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695475"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
directoryObjectId := "directoryObject-id"
graphClient.GroupsById(&groupId).MembersById(&directoryObjectId).$ref().Delete()


```