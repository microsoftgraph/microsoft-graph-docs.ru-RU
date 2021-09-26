---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4748f7f9f0583798007a48744e7d371052b17986901d394e5f7ceac036adc5be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57054856"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPCs = await graphClient.DeviceManagement.VirtualEndpoint.CloudPCs
    .Request()
    .GetAsync();

```