---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2a15421470b01db7be64ef4927a5c4ebfb0fe5e2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36360403"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOffice365GroupsActivityStorageCollectionPage getOffice365GroupsActivityStorage = graphClient.reports()
    .getOffice365GroupsActivityStorage("D7")
    .buildRequest()
    .get();

```