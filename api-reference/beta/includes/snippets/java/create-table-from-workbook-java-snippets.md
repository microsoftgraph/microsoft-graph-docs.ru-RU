---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 041f7f91bd423fa1d62f533a6216423bf602230d0f5eebbb7f37061c717f465a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141625"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String address = "A1:D8";

Boolean hasHeaders = false;

graphClient.me().drive().items("{id}").workbook().tables()
    .add(WorkbookTableAddParameterSet
        .newBuilder()
        .withAddress(address)
        .withHasHeaders(hasHeaders)
        .build())
    .buildRequest()
    .post();

```