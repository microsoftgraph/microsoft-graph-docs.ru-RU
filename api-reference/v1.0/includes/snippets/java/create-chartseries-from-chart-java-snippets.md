---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 51041d5fe7279ef30f1143163689b64ac64c31a0d78ebd0739a8f1e62de260b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57138067"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookChartSeries workbookChartSeries = new WorkbookChartSeries();
workbookChartSeries.name = "name-value";

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}").series()
    .buildRequest()
    .post(workbookChartSeries);

```