---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2b8fa71d457c03e8e32f628311b45d847bfd48a02aed2f896974ec0570ac8ae1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57371618"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var currentPassword = "xWwvJ]6NMw+bWH-d";

var newPassword = "0eM85N54wFxWwvJ]";

await graphClient.Me
    .ChangePassword(currentPassword,newPassword)
    .Request()
    .PostAsync();

```