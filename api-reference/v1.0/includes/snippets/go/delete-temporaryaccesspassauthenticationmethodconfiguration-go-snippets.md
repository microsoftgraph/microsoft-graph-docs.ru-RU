---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 81781bc138d20e067e95fc72fa1537c1f2cc41de
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094574"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

authenticationMethodConfigurationId := "authenticationMethodConfiguration-id"
graphClient.Policies().AuthenticationMethodsPolicy().AuthenticationMethodConfigurationsById(&authenticationMethodConfigurationId).Delete()


```