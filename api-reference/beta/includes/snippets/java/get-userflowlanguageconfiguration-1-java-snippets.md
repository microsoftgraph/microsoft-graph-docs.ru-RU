---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0dcab129380d75c6dfba0f660cadebac17a44f4729dc0ccf1f8362663a29cb0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57196799"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfigurationCollectionPage languages = graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp").languages()
    .buildRequest()
    .get();

```