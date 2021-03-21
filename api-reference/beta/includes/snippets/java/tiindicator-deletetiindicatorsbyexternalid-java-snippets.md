---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5034368f082b36b039403362820d8230f4c5efe6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973501"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> valueList = new LinkedList<String>();
valueList.add("externalId-value1");
valueList.add("externalId-value2");

graphClient.security().tiIndicators()
    .deleteTiIndicatorsByExternalId(TiIndicatorDeleteTiIndicatorsByExternalIdParameterSet
        .newBuilder()
        .withValue(valueList)
        .build())
    .buildRequest()
    .post();

```