---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 120a81d6af6929de65aa7ef5b021e795fe578f89
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618733"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var controls = await graphClient.Programs["673a7379-9c38-4f01-bd9d-4fda7260b807"].Controls
    .Request()
    .GetAsync();

```