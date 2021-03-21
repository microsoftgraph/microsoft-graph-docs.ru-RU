---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ab9db057d68ac06c048168f28e7a2ca4f6aa8489
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980941"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ReportRootGetCredentialUserRegistrationCountCollectionPage getCredentialUserRegistrationCount = graphClient.reports()
    .getCredentialUserRegistrationCount()
    .buildRequest()
    .get();

```