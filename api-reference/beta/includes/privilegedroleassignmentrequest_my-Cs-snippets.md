---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8ae0c4c61f0acb16c3e0ab108dc57b02f8f6f57d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443077"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var my = await graphClient.PrivilegedRoleAssignmentRequests.My()
    .Request()
    .GetAsync();

```