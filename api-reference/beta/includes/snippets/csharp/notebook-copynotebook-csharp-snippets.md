---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7af19f122901e1b7ab213989b9fd6e1a5f72a5fa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35488915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupId = "groupId-value";

var renameAs = "renameAs-value";

await graphClient.Me.Onenote.Notebooks["{id}"]
    .CopyNotebook(groupId,renameAs,notebookFolder,siteCollectionId,siteId)
    .Request()
    .PostAsync();

```