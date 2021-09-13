---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 22e520eb5fb5b4d5807ac7c83393ca53b55f26c439bb931ea7185708be3e64fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57367327"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Shares["{sharedDriveItem-id}"].DriveItem
    .Request()
    .Expand("children")
    .GetAsync();

```