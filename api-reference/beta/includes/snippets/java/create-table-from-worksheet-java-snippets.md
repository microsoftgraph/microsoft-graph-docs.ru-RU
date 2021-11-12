---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4172262567541510ac8a7b7f7e30e44326f296672768616efc1baf4c7a0be623
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57255959"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String address = "";

Boolean hasHeaders = false;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").tables()
    .add(WorkbookTableAddParameterSet
        .newBuilder()
        .withAddress(address)
        .withHasHeaders(hasHeaders)
        .build())
    .buildRequest()
    .post();

```