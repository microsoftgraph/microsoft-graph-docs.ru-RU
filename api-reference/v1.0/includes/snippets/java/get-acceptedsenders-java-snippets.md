---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6cb3df5fcafb44ffd2f0331ad82f82bc52b3ae1301eecfa6534c1b7cfd509612
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052403"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage acceptedSenders = graphClient.groups("{id}").acceptedSenders()
    .buildRequest()
    .get();

```