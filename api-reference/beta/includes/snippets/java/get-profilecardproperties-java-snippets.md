---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6ecb5302fdef7f04e84f59b2079d13a44e77e080
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968537"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IProfileCardPropertyCollectionPage profileCardProperties = graphClient.organization("{organizationId}").settings().profileCardProperties()
    .buildRequest()
    .get();

```