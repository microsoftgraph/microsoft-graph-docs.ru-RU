---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: faa291193cc074e09e0abfeabb11f5fa150e9e75
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971646"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageCatalogCollectionPage accessPackageCatalogs = graphClient.identityGovernance().entitlementManagement().accessPackageCatalogs()
    .buildRequest()
    .get();

```