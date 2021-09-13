---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2bfc1caf38a543e6a952886ff90d1433d2fabb638d5f14592f5669f3c00dd0d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143238"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Attachment attachment = graphClient.me().messages("AAMkADA1M-zAAA=").attachments("AAMkADA1M-CJKtzmnlcqVgqI=")
    .buildRequest()
    .get();

```