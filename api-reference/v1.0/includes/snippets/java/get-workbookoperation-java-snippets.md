---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: feeb87b502e7f464611003c931ce8f250eda7223106d991c6d6a57bdea25ba96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57256692"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookOperation workbookOperation = graphClient.me().drive().items("{drive-item-id}").workbook().operations("{operation-id}")
    .buildRequest()
    .get();

```