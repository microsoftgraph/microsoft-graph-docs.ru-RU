---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c91bb7f6990babff86185cb29a9d3aa61d00d13ff1371ebf4003c7225aef9a4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144731"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var issues = await graphClient.Admin.ServiceAnnouncement.Issues
    .Request()
    .GetAsync();

```