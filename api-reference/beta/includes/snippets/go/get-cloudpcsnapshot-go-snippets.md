---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 97d1a09475a22f89684ce6da94017284f3cd0f27
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341751"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

cloudPcSnapshotId := "cloudPcSnapshot-id"
result, err := graphClient.DeviceManagement().VirtualEndpoint().SnapshotsById(&cloudPcSnapshotId).Get()


```