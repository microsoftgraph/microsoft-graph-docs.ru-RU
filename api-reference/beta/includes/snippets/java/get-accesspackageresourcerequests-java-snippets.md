---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ccb67162ae1dcb71e7fdb5e252ac5a639ec26951
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951763"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IAccessPackageResourceRequestCollectionPage accessPackageResourceRequests = graphClient.identityGovernance().entitlementManagement().accessPackageResourceRequests()
    .buildRequest()
    .get();

```