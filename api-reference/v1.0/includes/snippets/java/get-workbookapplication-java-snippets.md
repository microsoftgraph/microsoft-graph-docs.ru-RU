---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e7515656517cd980eaacf7d87bb07096a63ede16a63c11766f2e29771fe9b737
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57430270"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookApplication workbookApplication = graphClient.me().drive().items("{id}").workbook().application()
    .buildRequest()
    .get();

```