---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 49b381d367d9a91f62a565247bc865f3785a2304
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717723"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedDriveItem = await graphClient.Shares["{shareIdOrEncodedSharingUrl}"]
    .Request()
    .GetAsync();

```