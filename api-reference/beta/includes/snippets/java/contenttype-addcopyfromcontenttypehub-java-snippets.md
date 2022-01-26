---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bf4f7f824d7b355b57c383e5f67f85b7c07397a4
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224789"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String contentTypeId = "String";

graphClient.sites("{siteId}").lists("{listId}").contentTypes()
    .addCopyFromContentTypeHub(ContentTypeAddCopyFromContentTypeHubParameterSet
        .newBuilder()
        .withContentTypeId(contentTypeId)
        .build())
    .buildRequest()
    .post();

```