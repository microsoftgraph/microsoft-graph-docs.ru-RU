---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 49b381d367d9a91f62a565247bc865f3785a2304
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618079"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedDriveItem = await graphClient.Shares["{shareIdOrEncodedSharingUrl}"]
    .Request()
    .GetAsync();

```