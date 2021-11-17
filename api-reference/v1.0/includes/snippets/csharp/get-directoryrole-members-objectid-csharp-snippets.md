---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2d935fc25c22764ad0b29134dfa352f1727693a9d81b46c5ef9efe1faf91892e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57257010"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.DirectoryRoles["{directoryRole-id}"].Members
    .Request()
    .GetAsync();

```