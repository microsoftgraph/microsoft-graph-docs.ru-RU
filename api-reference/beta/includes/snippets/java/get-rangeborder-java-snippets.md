---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cb4c59a818c2725c9e6d4050acc31c174be181c9c2400d9ae103601f4480ee9a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141725"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeBorder workbookRangeBorder = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().borders("{sideIndex}")
    .buildRequest()
    .get();

```