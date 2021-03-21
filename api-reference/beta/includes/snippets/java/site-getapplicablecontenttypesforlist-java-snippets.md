---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8057a3b0868062f9dd345ea56976c50915a4d541
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958980"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteGetApplicableContentTypesForListCollectionPage getApplicableContentTypesForList = graphClient.sites("{siteId}")
    .getApplicableContentTypesForList(SiteGetApplicableContentTypesForListParameterSet
        .newBuilder()
        .withListId("listId")
        .build())
    .buildRequest()
    .get();

```