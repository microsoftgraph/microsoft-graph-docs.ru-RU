---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f4a1f57e623d57af72d4674bf5adc9dc65ee354fb4acbcdbf880abbcf56e52c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57397466"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var parentReference = new ItemReference
{
    Id = "String"
};

var name = "String";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Restore(parentReference,name)
    .Request()
    .PostAsync();

```