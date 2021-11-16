---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f02efc61901654fc76b4ff2d0db22980daf910a1dc6ed802f8133028d33e1935
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57139678"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String id = "5793aa3b-cca9-4794-679a240f8b58";

graphClient.servicePrincipals("{id}")
    .getPasswordSingleSignOnCredentials(ServicePrincipalGetPasswordSingleSignOnCredentialsParameterSet
        .newBuilder()
        .withId(id)
        .build())
    .buildRequest()
    .post();

```