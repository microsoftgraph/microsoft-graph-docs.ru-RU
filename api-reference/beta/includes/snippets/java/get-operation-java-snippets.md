---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3555fc3590f0d2a4e2bf9cf44b1db09065c30a86e1b8310d56ef646c63699ecf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140571"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LongRunningOperation longRunningOperation = graphClient.users("{id | userPrincipalName}").authentication().operations("{id}")
    .buildRequest()
    .get();

```