---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2fd4a10342212ba5b51b2cd5b122db4b4c061eda
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968630"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LegalHold legalHold = new LegalHold();
legalHold.description = "This is a description for a legalHold";

graphClient.compliance().ediscovery().cases("{caseId}").legalHolds("{legalholdId}")
    .buildRequest()
    .patch(legalHold);

```