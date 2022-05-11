---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 50129d05d28bac324d2fc71bde4aab0513a47781
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315938"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String contentTypeId = "0x0101";

graphClient.sites("root").lists("Documents").contentTypes()
    .addCopyFromContentTypeHub(ContentTypeAddCopyFromContentTypeHubParameterSet
        .newBuilder()
        .withContentTypeId(contentTypeId)
        .build())
    .buildRequest()
    .post();

```