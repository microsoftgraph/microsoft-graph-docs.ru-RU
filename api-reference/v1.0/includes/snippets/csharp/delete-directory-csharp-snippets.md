---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ed831c7543d839f12e566de47a4965d8d8a045ba22228a76d0e4921eab728302
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57201195"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.DeletedItems["{directoryObject-id}"]
    .Request()
    .DeleteAsync();

```