---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8057a3b0868062f9dd345ea56976c50915a4d541
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59085001"
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