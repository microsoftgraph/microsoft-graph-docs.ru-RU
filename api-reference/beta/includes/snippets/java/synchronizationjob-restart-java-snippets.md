---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 63f429d779ba69be4910fb4b7533749cd7f611fd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967163"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Authorization", "Bearer <token>"));

SynchronizationJobRestartCriteria criteria = new SynchronizationJobRestartCriteria();
criteria.resetScope = EnumSet.of(SynchronizationJobRestartScope.WATERMARK,SynchronizationJobRestartScope.ESCROWS,SynchronizationJobRestartScope.QUARANTINE_STATE);

graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}")
    .restart(SynchronizationJobRestartParameterSet
        .newBuilder()
        .withCriteria(criteria)
        .build())
    .buildRequest( requestOptions )
    .post();

```