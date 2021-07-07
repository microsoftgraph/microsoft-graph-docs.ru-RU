---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a7a28d588eb22cc53c8b8b1c6ed0a41bc2b4008c
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316589"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var auditEvents = await graphClient.DeviceManagement.VirtualEndpoint.AuditEvents
    .Request()
    .GetAsync();

```