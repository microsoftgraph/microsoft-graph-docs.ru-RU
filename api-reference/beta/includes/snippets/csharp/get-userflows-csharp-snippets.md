---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e4b19ba4339caa6a51e86c921e992e5393b229fe1e787d03b2e400edfcbf7dd1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57306310"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlows = await graphClient.Identity.UserFlows
    .Request()
    .GetAsync();

```