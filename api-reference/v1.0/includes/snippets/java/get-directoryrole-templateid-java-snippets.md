---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1f5987544f20b578eee56df7319cea0ecd77e2b8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982413"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryRole directoryRole = graphClient.directoryRoles("roleTemplateId=4a5d8f65-41da-4de4-8968-e035b65339cf")
    .buildRequest()
    .get();

```