---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 677b3e6008a307133ccea25f31572fba8a071769
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966699"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EdiscoveryCase ediscoveryCase = new EdiscoveryCase();
ediscoveryCase.displayName = "My Case 1 - Renamed";
ediscoveryCase.description = "Updated description";
ediscoveryCase.externalId = "Updated externalId";

graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583")
    .buildRequest()
    .patch(ediscoveryCase);

```