---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d609cce137ee47f69d05273dd369c50c75a6eec9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65343241"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationUser()
displayName := "Rogelio Cazares"
requestBody.SetDisplayName(&displayName)
givenName := "Rogelio"
requestBody.SetGivenName(&givenName)
middleName := "Fernando"
requestBody.SetMiddleName(&middleName)
surname := "Cazares"
requestBody.SetSurname(&surname)
educationUserId := "educationUser-id"
graphClient.Education().UsersById(&educationUserId).Patch(requestBody)


```