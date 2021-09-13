---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 20a35833c96f58f60e5fb72b00ac390915d841ad70164f80b1ba1c70bc266356
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57311179"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage appliesTo = graphClient.policies().claimsMappingPolicies("{id}").appliesTo()
    .buildRequest()
    .get();

```