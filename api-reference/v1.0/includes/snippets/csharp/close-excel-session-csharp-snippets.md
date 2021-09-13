---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4d03fda7142f21080a8e67ee151ff7fdd1d4991058ebe77f0017065343c2bc1c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57212840"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook
    .CloseSession()
    .Request()
    .Header("workbook-session-id","{session-id}")
    .PostAsync();

```