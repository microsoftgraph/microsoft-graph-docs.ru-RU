---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 824b684e1d37c399edcda835f01f462f956ea7fa
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177147"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permission = await graphClient.Sites["{sitesId}"].Permissions["{permissionId}"]
    .Request()
    .GetAsync();

```