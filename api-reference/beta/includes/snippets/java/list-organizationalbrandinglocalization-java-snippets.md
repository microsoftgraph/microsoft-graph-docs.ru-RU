---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8e9769bfa2e1538673a5c9a6915ed814a757a19e
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995523"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBrandingLocalizationCollectionPage localizations = graphClient.organization("84841066-274d-4ec0-a5c1-276be684bdd3").branding().localizations()
    .buildRequest()
    .get();

```