---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d7ee14a45ffd3727d12e321ce9a04e6689f3e252
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979841"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeBorder workbookRangeBorder = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().borders("{sideIndex}")
    .buildRequest()
    .get();

```