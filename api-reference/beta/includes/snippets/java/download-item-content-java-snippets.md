---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e112f4070e288cede7e75cc7d4d482beb4004d7f7cd8789e70a202a1f40df06c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140915"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/me/drive/items/{item-id}/content", InputStream.class)
    .buildRequest()
    .get();

```