---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 258dbe36a3fae7323aec048ff15f1876d4342667
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969829"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = new AdministrativeUnit();
administrativeUnit.displayName = "Seattle District Technical Schools";
administrativeUnit.description = "Seattle district technical schools administration";
administrativeUnit.visibility = "HiddenMembership";

graphClient.directory().administrativeUnits()
    .buildRequest()
    .post(administrativeUnit);

```