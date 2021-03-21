---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b2af29f8bc38519f757ac54e07390e64d4344e6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970939"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UUID keyId = UUID.fromString("f0b0b335-1d71-4883-8f98-567911bfdca6");

String proof = "eyJ0eXAiOiJ...";

graphClient.servicePrincipals("{id}")
    .removeKey(ServicePrincipalRemoveKeyParameterSet
        .newBuilder()
        .withKeyId(keyId)
        .withProof(proof)
        .build())
    .buildRequest()
    .post();

```