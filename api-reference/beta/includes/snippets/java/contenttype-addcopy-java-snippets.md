---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b8d261117b7962ff4c5a48767402574436aa8575
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "60729439"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String contentType = "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101";

graphClient.sites("{site-id}").lists("{list-id}").contentTypes()
    .addCopy(ContentTypeAddCopyParameterSet
        .newBuilder()
        .withContentType(contentType)
        .build())
    .buildRequest()
    .post();

```