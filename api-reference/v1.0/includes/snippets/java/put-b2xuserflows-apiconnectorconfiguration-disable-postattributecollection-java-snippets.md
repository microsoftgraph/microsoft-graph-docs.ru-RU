---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f5d04916aaaf706c91df0474d47d002e4288edadb923b6a7f365fc2fc9f3658d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141471"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityApiConnector identityApiConnector = new IdentityApiConnector();

graphClient.identity().b2xUserFlows("B2X_1_testuserflow").postAttributeCollection().reference()
    .buildRequest()
    .put(identityApiConnector);

```