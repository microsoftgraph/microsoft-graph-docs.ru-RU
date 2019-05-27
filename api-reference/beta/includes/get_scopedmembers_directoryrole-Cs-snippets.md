---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 55a6388a33c0c5d7687550fccbc2d7e09fb3d4e0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446486"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedMembers = await graphClient.DirectoryRoles["{id}"].ScopedMembers
    .Request()
    .GetAsync();

```