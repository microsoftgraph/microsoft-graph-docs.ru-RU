---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: adfe5779991261700ca598872c06bac2e929f41f85fda3d64c950e10179eab7d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143031"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Admin.ServiceAnnouncement.Messages
    .Request()
    .GetAsync();

```