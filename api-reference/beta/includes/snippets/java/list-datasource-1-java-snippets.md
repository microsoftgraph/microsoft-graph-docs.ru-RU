---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 21d012ade8f778d816fed53f2d911b8c14129fda43090acb85a1b0316d262591
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57203153"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DataSourceCollectionPage additionalSources = graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("{sourceCollectionId}").additionalSources()
    .buildRequest()
    .get();

```