---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a08690a4a2ede314d65239d50007f22bdedf40da08fa55c2c62b40786a3a0066
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57372586"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var administrativeUnit = await graphClient.Directory.AdministrativeUnits["{administrativeUnit-id}"]
    .Request()
    .GetAsync();

```