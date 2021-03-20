---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3f5932036305a7562171208d14be7f1bc06ec6b0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972494"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CertificateBasedAuthConfiguration certificateBasedAuthConfiguration = new CertificateBasedAuthConfiguration();
LinkedList<CertificateAuthority> certificateAuthoritiesList = new LinkedList<CertificateAuthority>();
CertificateAuthority certificateAuthorities = new CertificateAuthority();
certificateAuthorities.isRootAuthority = true;
certificateAuthorities.certificate = Base64.getDecoder().decode("Binary");
certificateAuthoritiesList.add(certificateAuthorities);
certificateBasedAuthConfiguration.certificateAuthorities = certificateAuthoritiesList;

graphClient.organization("{id}").certificateBasedAuthConfiguration()
    .buildRequest()
    .post(certificateBasedAuthConfiguration);

```