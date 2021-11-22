---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b1e37f0a6afcb2a52180ab67382b3bc3d257740df1876285f4f1ddd9b697d16d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57256002"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WebAccount webAccount = graphClient.me().profile().webAccounts("{id}")
    .buildRequest()
    .get();

```