---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7b5c39a0dcb9b6f25b5abdcd3ba6f32d79de7255
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339793"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcSnapshotId = "A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8";

await graphClient.DeviceManagement.ManagedDevices["{managedDevice-id}"]
    .RestoreCloudPc(cloudPcSnapshotId)
    .Request()
    .PostAsync();

```