---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b257ffb2ac0213b14f537ee2a308151714df7374
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969807"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "My custom name";

graphClient.applicationTemplates("{id}")
    .instantiate(ApplicationTemplateInstantiateParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .build())
    .buildRequest()
    .post();

```