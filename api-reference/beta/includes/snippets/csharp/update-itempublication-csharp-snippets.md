---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3fb63ee509a41decd0d25656971e7636a639514dd453e3faa50dc5330f2e9ddd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57322562"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPublication = new ItemPublication
{
    Publisher = "International Association of Branding Management Publishing",
    ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
};

await graphClient.Users["{user-id}"].Profile.Publications["{itemPublication-id}"]
    .Request()
    .UpdateAsync(itemPublication);

```