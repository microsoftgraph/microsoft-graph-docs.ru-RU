---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 55336fbba8544dd7f9d9fa9f2a5895aaeba63ab6
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573654"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectionOperation = await graphClient.Connections["{externalConnectors.externalConnection-id}"].Operations["{externalConnectors.connectionOperation-id}"]
    .Request()
    .GetAsync();

```