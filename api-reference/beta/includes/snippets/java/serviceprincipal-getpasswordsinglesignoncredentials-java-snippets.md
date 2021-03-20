---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3eff6bef2936323c6a55bb4986ae15862520e5d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976057"
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