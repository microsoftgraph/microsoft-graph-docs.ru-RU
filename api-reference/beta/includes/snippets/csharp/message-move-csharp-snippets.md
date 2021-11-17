---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4eaa99f700470249ba937c230fda4cda1dda0bce89341b46c3bf3851b7c75546
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57252182"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "deleteditems";

await graphClient.Me.Messages["{message-id}"]
    .Move(destinationId)
    .Request()
    .PostAsync();

```