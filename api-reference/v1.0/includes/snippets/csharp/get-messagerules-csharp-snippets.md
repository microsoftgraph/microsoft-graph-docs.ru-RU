---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fba5222968d25e04bd53e804fe520a742dbda154
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35704939"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageRules = await graphClient.Me.MailFolders["inbox"].MessageRules
    .Request()
    .GetAsync();

```