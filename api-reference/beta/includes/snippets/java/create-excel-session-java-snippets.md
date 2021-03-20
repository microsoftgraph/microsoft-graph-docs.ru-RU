---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 569aae23d8f712c3e02f4f541df358188e8746f0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970616"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean persistChanges = true;

graphClient.me().drive().items("{id}").workbook()
    .createSession(WorkbookCreateSessionParameterSet
        .newBuilder()
        .withPersistChanges(persistChanges)
        .build())
    .buildRequest()
    .post();

```