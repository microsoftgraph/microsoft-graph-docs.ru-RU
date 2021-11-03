---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 863c776c9e4f53003724aece2cc1b0ee88bd8345
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688593"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = new Device
{
    ExtensionAttributes = new OnPremisesExtensionAttributes
    {
        ExtensionAttribute1 = "BYOD-Device"
    }
};

await graphClient.Devices["{device-id}"]
    .Request()
    .UpdateAsync(device);

```