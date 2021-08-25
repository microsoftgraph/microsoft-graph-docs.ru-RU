---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1a1970af42450fe92c9eca37bb88047b0c7ce915ef0ecf3b78296e799be0a88d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57262128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversations = await graphClient.Groups["{group-id}"].Conversations
    .Request()
    .GetAsync();

```