---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d545be5f0c0c1713505ff2d97a8a09c736cfb395
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116577"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.bookingBusinesses("Contosolunchdelivery@contoso.onmicrosoft.com").appointments("AAMkADKqAAA=")
    .buildRequest()
    .delete();

```