---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0734d823dd7cd4bfb81e3743e04026d6ec0d6547692a739dceeb7908e8c61569
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57264894"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = new ServicePrincipal();
servicePrincipal.appId = "65415bb1-9267-4313-bbf5-ae259732ee12";

graphClient.servicePrincipals()
    .buildRequest()
    .post(servicePrincipal);

```