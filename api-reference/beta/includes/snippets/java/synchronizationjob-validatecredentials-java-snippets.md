---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fff12ef7a7ddcd44f26e77754deb02fdb248291b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970733"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<SynchronizationSecretKeyStringValuePair> credentialsList = new LinkedList<SynchronizationSecretKeyStringValuePair>();
SynchronizationSecretKeyStringValuePair credentials = new SynchronizationSecretKeyStringValuePair();
credentials.key = SynchronizationSecret.USER_NAME;
credentials.value = "user@domain.com";

credentialsList.add(credentials);
SynchronizationSecretKeyStringValuePair credentials1 = new SynchronizationSecretKeyStringValuePair();
credentials1.key = SynchronizationSecret.PASSWORD;
credentials1.value = "password-value";

credentialsList.add(credentials1);

graphClient.servicePrincipals("{id}").synchronization().jobs("{id}")
    .validateCredentials(SynchronizationJobValidateCredentialsParameterSet
        .newBuilder()
        .withApplicationIdentifier(null)
        .withTemplateId(null)
        .withUseSavedCredentials(null)
        .withCredentials(credentialsList)
        .build())
    .buildRequest()
    .post();

```