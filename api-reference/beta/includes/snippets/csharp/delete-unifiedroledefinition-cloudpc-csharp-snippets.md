---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 55ed944b76dd01882f2fc1eb1cd9ae425a1a7dcb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089294"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.RoleManagement.CloudPC.RoleDefinitions["{unifiedRoleDefinition-id}"]
    .Request()
    .DeleteAsync();

```