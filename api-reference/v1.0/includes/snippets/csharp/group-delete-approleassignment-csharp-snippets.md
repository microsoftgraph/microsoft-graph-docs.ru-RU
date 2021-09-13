---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9c4d86e69c8e1aefa0c6e6bc57683a131cf9fe0c81dbc41fbf5913aed27652f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57366938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{group-id}"].AppRoleAssignments["{appRoleAssignment-id}"]
    .Request()
    .DeleteAsync();

```