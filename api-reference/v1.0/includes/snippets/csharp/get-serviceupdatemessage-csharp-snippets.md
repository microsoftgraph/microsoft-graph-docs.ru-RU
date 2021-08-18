---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a97aea0b77aae18f3a53e91710a49790d645c95a
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58258020"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var serviceUpdateMessage = await graphClient.Admin.ServiceAnnouncement.Messages["{serviceUpdateMessage-id}"]
    .Request()
    .GetAsync();

```