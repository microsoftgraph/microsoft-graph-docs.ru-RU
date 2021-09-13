---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7d9cea2ea0f859154fafce47a8c65c15b13f68e9415f384ea494f010192dd6bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57395112"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().administrativeUnits("{id}").scopedRoleMembers("{id}")
    .buildRequest()
    .delete();

```