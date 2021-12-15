---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f283e6153ddc6155c854919888567d8ce9645b58
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525478"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content tasks = graphClient.me().tasks().lists().aQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNm().tasks()
    .buildRequest()
    .get();

```