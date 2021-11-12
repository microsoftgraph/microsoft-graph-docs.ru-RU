---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bbd40fc01baebb31b01ecb722589f9ec5e32252556e6d7257908debf7d74e4e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57318810"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.drive().root().workbook().worksheets("{id}")
    .range()
    .columnsBefore(WorkbookRangeColumnsBeforeParameterSet
        .newBuilder()
        .withCount(2)
        .build())
    .buildRequest()
    .get();

```