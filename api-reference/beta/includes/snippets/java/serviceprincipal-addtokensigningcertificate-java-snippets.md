---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 475c55d54405a571b4b99b7e9bb2e32670023c31
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202528"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "CN=customDisplayName";

OffsetDateTime endDateTime = OffsetDateTimeSerializer.deserialize("01/25/2024 00:00:00");

graphClient.servicePrincipals("7c8d4399-b4bf-413a-8b6a-c577790cae7d")
    .addTokenSigningCertificate(ServicePrincipalAddTokenSigningCertificateParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .withEndDateTime(endDateTime)
        .build())
    .buildRequest()
    .post();

```