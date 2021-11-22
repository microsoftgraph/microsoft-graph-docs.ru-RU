---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f92ebc220f00ea58225330a6dd398958abe3bd7787ad28d3275f26100449594e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57247675"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connections = await graphClient.External.Connections
    .Request()
    .GetAsync();

```