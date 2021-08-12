---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: de9dae2c022181e17dfcc6c870dfd58b2dca6c39de45d90e74b302bc737d0838
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129796"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADADVj3fyAABZ5hYdAAA="]
    .Request()
    .Expand("eventMessage/event")
    .GetAsync();

```