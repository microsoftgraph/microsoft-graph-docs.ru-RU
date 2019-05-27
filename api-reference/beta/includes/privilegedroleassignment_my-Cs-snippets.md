---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e21d42b603dc529118e69f0fce1ddafd59edd3e0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443140"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var my = await graphClient.PrivilegedRoleAssignments.My()
    .Request()
    .GetAsync();

```