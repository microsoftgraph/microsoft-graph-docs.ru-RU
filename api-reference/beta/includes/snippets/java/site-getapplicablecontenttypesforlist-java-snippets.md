---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3df22a6c1aeb07ab1d2b8617c271b3a7c9ad91ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772431"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteGetApplicableContentTypesForListCollectionPage getApplicableContentTypesForList = graphClient.sites("{siteId}")
    .getApplicableContentTypesForList("listId")
    .buildRequest()
    .get();

```