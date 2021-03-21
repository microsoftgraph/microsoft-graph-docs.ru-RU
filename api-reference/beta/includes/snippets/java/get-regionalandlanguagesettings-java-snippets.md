---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1523dbe46baf187ec31d93f36a03b9be9c16829d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970586"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RegionalAndLanguageSettings regionalAndLanguageSettings = graphClient.me().settings().regionalAndLanguageSettings()
    .buildRequest()
    .get();

```