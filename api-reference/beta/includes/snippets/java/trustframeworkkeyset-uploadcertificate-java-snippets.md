---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 75fb68f02404870ac327aa62cc3a984094c89fe8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980617"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String key = "key-value";

graphClient.trustFramework().keySets("{id}")
    .uploadCertificate(TrustFrameworkKeySetUploadCertificateParameterSet
        .newBuilder()
        .withKey(key)
        .build())
    .buildRequest()
    .post();

```