---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dc511aaeb2df987a4bc4a734886d8b61444b65895902f0cf3d9fd33dc2d4e86f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57248473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organizationalBranding = await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .GetAsync();

```