---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 437b1b0cec3ac4d6239020a7d8bbcbdba70e6c45603b610ceb15192501e03a25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57368735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["{message-id}"]
    .Request()
    .Select("internetMessageHeaders")
    .GetAsync();

```