---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ed9936994dcba50677cdf9bcf9c7837b2a03eea4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979196"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationTemplate synchronizationTemplate = new SynchronizationTemplate();
synchronizationTemplate.id = "SCIM-Test1";
synchronizationTemplate.applicationId = UUID.fromString("{id}");
synchronizationTemplate.factoryTag = "CustomSCIM";

graphClient.applications("{id}").synchronization().templates()
    .buildRequest()
    .post(synchronizationTemplate);

```