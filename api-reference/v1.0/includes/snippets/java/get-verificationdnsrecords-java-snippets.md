---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1d467eb464eda2aae6351963b9aa12e5b2292024
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979637"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DomainDnsRecordCollectionPage verificationDnsRecords = graphClient.domains("{domain-name}").verificationDnsRecords()
    .buildRequest()
    .get();

```