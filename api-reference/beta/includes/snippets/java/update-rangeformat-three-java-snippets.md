---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c44fddc34993db9435f914b95b5d094a6d427bdf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976088"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeFormat workbookRangeFormat = new WorkbookRangeFormat();
workbookRangeFormat.columnWidth = 135d;
workbookRangeFormat.horizontalAlignment = "Right";
workbookRangeFormat.verticalAlignment = "Top";
workbookRangeFormat.rowHeight = 49d;
workbookRangeFormat.wrapText = false;

graphClient.me().drive().items("{id}").workbook().worksheets("Sheet1")
    .range("$C$1").format()
    .buildRequest()
    .patch(workbookRangeFormat);

```