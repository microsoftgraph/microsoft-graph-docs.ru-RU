---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5d53e74d5f0809c9e76ded799e1b5ff8b7e517a0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969955"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Domain domain = new Domain();
domain.isDefault = true;
LinkedList<String> supportedServicesList = new LinkedList<String>();
supportedServicesList.add("Email");
supportedServicesList.add("OfficeCommunicationsOnline");
domain.supportedServices = supportedServicesList;

graphClient.domains("contoso.com")
    .buildRequest()
    .patch(domain);

```