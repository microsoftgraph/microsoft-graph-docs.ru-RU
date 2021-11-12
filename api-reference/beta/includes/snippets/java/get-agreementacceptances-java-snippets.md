---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 42d729c6c204ae5c0acf318fb3bf0cc95397550a9b3751c4137aaf7ff20556e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271422"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AgreementAcceptanceCollectionWithReferencesPage agreementAcceptances = graphClient.me().agreementAcceptances()
    .buildRequest()
    .get();

```