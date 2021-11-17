---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 255b826a5dd71e7e79df070fdb4b4b3358ae1adbe1c02f348889d55fe19436e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144385"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("fd15cad8-80f6-484f-9666-3caf695fbf32").schedule().timeCards("TCK_cc09588d-d9d2-4fa0-85dc-2aa5ef983972")
    .confirm()
    .buildRequest()
    .post();

```