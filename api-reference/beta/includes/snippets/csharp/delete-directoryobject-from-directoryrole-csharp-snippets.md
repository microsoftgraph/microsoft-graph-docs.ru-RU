---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1e3421b9bf527a2f6293a6c45e7861e71d79dc90ef54ac588badaddd00ca5174
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57316662"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DirectoryRoles["{directoryRole-id}"].Members["{directoryObject-id}"].Reference
    .Request()
    .DeleteAsync();

```