---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff2cf2aa1321b4256c698d4fe13ae0afa7113888
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794756"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directorySettingTemplate = await graphClient.DirectorySettingTemplates["{directorySettingTemplate-id}"]
    .Request()
    .GetAsync();

```