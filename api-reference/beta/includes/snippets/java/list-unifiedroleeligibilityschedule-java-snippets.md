---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7ac2437d904658bdcde102407c14215ec7f679d5f00750a1effd7bc544adcf94
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57196099"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleCollectionPage roleEligibilitySchedules = graphClient.roleManagement().directory().roleEligibilitySchedules()
    .buildRequest()
    .get();

```