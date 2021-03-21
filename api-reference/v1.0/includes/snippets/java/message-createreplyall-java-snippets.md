---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 21fbdd058f27fa812b320c5edeedda27eae2aecf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977471"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .createReplyAll(MessageCreateReplyAllParameterSet
        .newBuilder()
        .withMessage(null)
        .withComment(null)
        .build())
    .buildRequest()
    .post();

```