---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1f54f171da952555e55dc7f1de1770f3aa9bbb6f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972076"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationId = "destinationId-value";

graphClient.me().messages("{id}")
    .copy(MessageCopyParameterSet
        .newBuilder()
        .withDestinationId(destinationId)
        .build())
    .buildRequest()
    .post();

```