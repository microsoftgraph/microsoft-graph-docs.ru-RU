---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f243d0b5ba3e3aeef1bb31a75fffa6afed363ab0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972059"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemEmail itemEmail = new ItemEmail();
itemEmail.address = "Innocenty.Popov@adventureworks.com";

graphClient.me().profile().emails()
    .buildRequest()
    .post(itemEmail);

```