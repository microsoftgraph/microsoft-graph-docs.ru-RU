---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 17246b23984da0e8dd5bf5b3eee5a42f4504a109a5d2bc96a26b3a00e6ea699a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57196798"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfigurationCollectionPage languages = graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp").languages()
    .buildRequest()
    .filter("isEnabled eq true")
    .get();

```