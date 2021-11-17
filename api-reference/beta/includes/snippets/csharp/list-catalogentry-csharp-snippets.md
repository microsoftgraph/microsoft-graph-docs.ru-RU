---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7d4dbf851196d2d9cdf806ff931b1b8fe8d13771e72df209c034ee7135cc6fd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57306917"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entries = await graphClient.Admin.Windows.Updates.Catalog.Entries
    .Request()
    .GetAsync();

```