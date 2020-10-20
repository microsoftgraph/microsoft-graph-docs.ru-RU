---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 98e625b910e4df40952a545b05b9b5e4ce24bb61
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620441"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySettingTemplates = await graphClient.DirectorySettingTemplates
    .Request()
    .GetAsync();

```