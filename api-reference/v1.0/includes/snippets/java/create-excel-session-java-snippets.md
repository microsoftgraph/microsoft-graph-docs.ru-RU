---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a20c6688fcd962247049fa2873a2942be5460d2f4e63726cfc141da3659ae48e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57397595"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean persistChanges = true;

graphClient.me().drive().items("{id}").workbook()
    .createSession(WorkbookCreateSessionParameterSet
        .newBuilder()
        .withPersistChanges(persistChanges)
        .build())
    .buildRequest()
    .post();

```