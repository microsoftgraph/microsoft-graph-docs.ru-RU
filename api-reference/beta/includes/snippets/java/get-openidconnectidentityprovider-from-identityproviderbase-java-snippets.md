---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 96c1b95c05356f441f0a32dd0d6617664ead6901728fe9f9dd28106fd73b9f8f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57320448"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBase identityProviderBase = graphClient.identity().identityProviders("OIDC-V1-test-icm-4470de58-86c2-4a3f-a22c-63c9366cd000")
    .buildRequest()
    .get();

```