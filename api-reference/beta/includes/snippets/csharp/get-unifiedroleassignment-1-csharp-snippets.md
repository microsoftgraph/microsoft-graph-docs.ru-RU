---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1af61a37e05ea47a1d7cec79a72455e3c8999180a433cfb53ca1bf0ee62958a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57202677"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = await graphClient.RoleManagement.Directory.RoleAssignments["{unifiedRoleAssignment-id}"]
    .Request()
    .GetAsync();

```