---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 60eacc27cfc9a64e4d502a60a6368708dae7aa55
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976102"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = new Subscription();
subscription.expirationDateTime = OffsetDateTimeSerializer.deserialize("2016-11-22T18:23:45.9356913Z");

graphClient.subscriptions("{id}")
    .buildRequest()
    .patch(subscription);

```