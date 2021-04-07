---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1072f3da89344c07883d25b6cef2e8c75d86ae23
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611963"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Chats["{chat-id}"].Messages
    .Request()
    .Top(2)
    .GetAsync();

```