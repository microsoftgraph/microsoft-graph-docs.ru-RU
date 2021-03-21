---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 825efe0e5112d7195f25c2eae4be13be8cadf906
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981876"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SourceCollection sourceCollection = new SourceCollection();
sourceCollection.displayName = "Quarterly Financials search";

graphClient.compliance().ediscovery().cases("{caseId}").sourceCollections("1a9b4145d8f84e39bc45a7f68c5c5119")
    .buildRequest()
    .patch(sourceCollection);

```