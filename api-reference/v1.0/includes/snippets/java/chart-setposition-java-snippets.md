---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 29d46835515ea8e1dbcb7be1e0370ac1df91c3be
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975432"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

JsonElement startCell = JsonParser.parseString("startCell-value");

JsonElement endCell = JsonParser.parseString("endCell-value");

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}")
    .setPosition(WorkbookChartSetPositionParameterSet
        .newBuilder()
        .withStartCell(startCell)
        .withEndCell(endCell)
        .build())
    .buildRequest()
    .post();

```