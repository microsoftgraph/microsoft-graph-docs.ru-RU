---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3b2aea2fcb556be7fe408d75b3bbc6d3a5ffcf15
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793532"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.SchemaExtensions["{schemaExtension-id}"]
    .Request()
    .DeleteAsync();

```