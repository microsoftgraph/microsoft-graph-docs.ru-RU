---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e2a49f439fa6b85ef15666a14b7eab62a5dc6c4f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005528"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
connectorId := "connector-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).ConnectorsById(&connectorId).MemberOf().Get(options)


```