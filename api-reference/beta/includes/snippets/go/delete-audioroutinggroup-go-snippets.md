---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 80b7c3e7ef6d4081fc8a43ae08c7c288f2989ef6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341657"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
audioRoutingGroupId := "audioRoutingGroup-id"
graphClient.Communications().CallsById(&callId).AudioRoutingGroupsById(&audioRoutingGroupId).Delete()


```