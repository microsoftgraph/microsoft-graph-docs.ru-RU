---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a7db7f38bb2c93ad1307aebdae23cc9113b3d0524c7a006ebfa0229d0748b01f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57212741"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcAuditEvent = await graphClient.DeviceManagement.VirtualEndpoint.AuditEvents["{cloudPcAuditEvent-id}"]
    .Request()
    .GetAsync();

```