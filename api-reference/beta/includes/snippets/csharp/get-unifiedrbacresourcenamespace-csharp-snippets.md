---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5841133249661c80570efb69e25bbce848cf1218
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63339809"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRbacResourceNamespace = await graphClient.RoleManagement.Directory.ResourceNamespaces["{unifiedRbacResourceNamespace-id}"]
    .Request()
    .GetAsync();

```