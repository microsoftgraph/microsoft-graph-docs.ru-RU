---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 19b6887d8ba1c5c1ba74cf50dc62d27cc31f67ef893d06a28fa00215e2bc35a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57372410"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var response = await graphClient.Me.Drive.Items["{driveItem-id}"].Thumbnails["{thumbnailSet-id}"]["{thumbnailSet-id}"]
    .Request()
    .GetAsync();

```