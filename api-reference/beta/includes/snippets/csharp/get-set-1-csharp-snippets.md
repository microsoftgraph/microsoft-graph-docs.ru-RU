---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0c8a9c273238f67c7e32615ad3ae7b91b464ac4ff148b27f955def80b27e0dcd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57313945"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sets = await graphClient.TermStore.Groups["{termStore.group-id}"].Sets
    .Request()
    .GetAsync();

```