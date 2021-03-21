---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aef65a6584056ebd508c849ca9332c7e1bac1813
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979477"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartTitle workbookChartTitle = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").title()
    .buildRequest()
    .get();

```