---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5d833b357aafbdb88eb518f16c68109b4774f9ad
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619090"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var thumbnails = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails
    .Request()
    .GetAsync();

```