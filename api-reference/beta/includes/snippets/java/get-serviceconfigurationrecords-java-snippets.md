---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 29203eb354bf5bef9492c69ac457b36aaa020e29
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956015"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDomainDnsRecordCollectionPage serviceConfigurationRecords = graphClient.domains("contoso.com").serviceConfigurationRecords()
    .buildRequest()
    .get();

```