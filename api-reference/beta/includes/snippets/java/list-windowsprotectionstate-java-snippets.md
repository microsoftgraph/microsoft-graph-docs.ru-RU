---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1bb40f86c93ffcd7b208394097a6718d8dd69324cd104c3188514b026b9f253e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143092"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WindowsProtectionStateCollectionPage windowsProtectionStates = graphClient.tenantRelationships().managedTenants().windowsProtectionStates()
    .buildRequest()
    .get();

```