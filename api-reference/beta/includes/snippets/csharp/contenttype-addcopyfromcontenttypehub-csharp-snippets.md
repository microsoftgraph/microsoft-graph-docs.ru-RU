---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c6c5bc7348d93a985333ca54cb36541b00a3e45d
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224781"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentTypeId = "String";

await graphClient.Sites["{site-id}"].Lists["{list-id}"].ContentTypes
    .AddCopyFromContentTypeHub(contentTypeId)
    .Request()
    .PostAsync();

```