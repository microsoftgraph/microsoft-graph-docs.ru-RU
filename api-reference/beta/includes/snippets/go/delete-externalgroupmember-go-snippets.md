---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e783c0e53fb2c3477cbe03c8a100b19a74047370
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340210"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
externalGroupId := "externalGroup-id"
identityId := "identity-id"
graphClient.External().ConnectionsById(&externalConnectionId).GroupsById(&externalGroupId).MembersById(&identityId).Delete()


```