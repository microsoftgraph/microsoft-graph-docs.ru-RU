---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cc38b6ed14f200d5639f65b84a1cc8338f25748c
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528782"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

externalConnectionId := "externalConnection-id"
externalGroupId := "externalGroup-id"
identityId := "identity-id"
graphClient.External().ConnectionsById(&externalConnectionId).GroupsById(&externalGroupId).MembersById(&identityId).Delete(nil)


```