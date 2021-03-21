---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5c3f6fcff328af9db92e7eda1625e23919f5a392
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973367"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean isSyncedFromOnPremises = false;

graphClient.directoryObjects()
    .getAvailableExtensionProperties(DirectoryObjectGetAvailableExtensionPropertiesParameterSet
        .newBuilder()
        .withIsSyncedFromOnPremises(isSyncedFromOnPremises)
        .build())
    .buildRequest()
    .post();

```