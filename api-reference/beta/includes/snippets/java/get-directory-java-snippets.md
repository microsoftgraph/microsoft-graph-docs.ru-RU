---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a0e0f3101258aebee5183a2961ced1375ef41e0eece3ed10673f874215f30483
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57266496"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directory().deletedItems("46cc6179-19d0-473e-97ad-6ff84347bbbb")
    .buildRequest()
    .get();

```