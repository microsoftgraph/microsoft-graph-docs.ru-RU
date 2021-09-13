---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f4dceeb324cb53e7cbcd93d362f3455e5440bd9d6c3e73cfcee0943683ba459b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57396850"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .cell(WorkbookRangeCellParameterSet
        .newBuilder()
        .withRow(5)
        .withColumn(6)
        .build())
    .buildRequest()
    .get();

```