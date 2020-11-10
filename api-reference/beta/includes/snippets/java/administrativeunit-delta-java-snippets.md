---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8ec6a0b3eeec77e600b33bc77fa8cd2375c2b5e5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962685"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAdministrativeUnitDeltaCollectionPage delta = graphClient.administrativeUnits()
    .delta()
    .buildRequest()
    .get();

```