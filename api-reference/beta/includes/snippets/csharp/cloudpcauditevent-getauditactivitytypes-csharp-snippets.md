---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fa57b89ecf0146a4425a8bf3ad71da7bfe955883c9a8e44b0a25c03b43fe10e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57195595"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAuditActivityTypes = await graphClient.DeviceManagement.VirtualEndpoint.AuditEvents
    .GetAuditActivityTypes()
    .Request()
    .GetAsync();

```