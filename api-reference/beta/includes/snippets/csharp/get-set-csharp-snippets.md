---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 974762d339c70a7ecd5be7bad780feffbdb0a3ec
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015308"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sets = await graphClient.TermStore.Groups["{groupId}"].Sets
    .Request()
    .GetAsync();

```