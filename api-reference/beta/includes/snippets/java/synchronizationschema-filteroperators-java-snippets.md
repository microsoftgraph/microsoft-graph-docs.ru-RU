---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8a4d464131674f8d8f4fb1137233ec1927593ae2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980894"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationSchemaFilterOperatorsCollectionPage filterOperators = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema()
    .filterOperators()
    .buildRequest()
    .get();

```