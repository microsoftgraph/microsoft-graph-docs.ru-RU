---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5c3dd8ab3fa3501e27b22b32c733d58ca7a22ae5987fb3c795fb677af8303dfd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57211083"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleSchedules = await graphClient.RoleManagement.Directory
    .RoleSchedules("a3bb8764-cb92-4276-9d2a-ca1e895e55ea","a3bb8764-cb92-4276-9d2a-ca1e895e55ea","a3bb8764-cb92-4276-9d2a-ca1e895e55ea","a3bb8764-cb92-4276-9d2a-ca1e895e55ea")
    .Request()
    .GetAsync();

```