---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 53660eab808981d3e55e3219c83895fae1ae2481082658ea0c681fe777b62cee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57311146"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryRoles = await graphClient.DirectoryRoles
    .Request()
    .GetAsync();

```