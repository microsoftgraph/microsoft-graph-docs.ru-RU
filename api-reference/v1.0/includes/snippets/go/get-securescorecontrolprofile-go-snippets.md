---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2f57b700b19a8d1bc49c8b5fc3a05b4105f0bcec
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61295191"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

secureScoreControlProfileId := "secureScoreControlProfile-id"
result, err := graphClient.Security().SecureScoreControlProfilesById(&secureScoreControlProfileId).Get(nil)


```