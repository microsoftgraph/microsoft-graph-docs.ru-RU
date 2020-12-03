---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d13cb4309e584f915c118982dc418624b6b365e1
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524533"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["d69179bf-f4a4-41a9-a9de-249c0f2efb1d"].Branding.Localizations["fr"]
    .Request()
    .DeleteAsync();

```