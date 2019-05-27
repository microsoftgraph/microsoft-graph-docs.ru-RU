---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 98e625b910e4df40952a545b05b9b5e4ce24bb61
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471868"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySettingTemplates = await graphClient.DirectorySettingTemplates
    .Request()
    .GetAsync();

```