---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0b1ac9e73ec9b29b112ad832bbb35712edd4a2a6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59073880"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBaseAvailableProviderTypesCollectionPage availableProviderTypes = graphClient.identity().identityProviders()
    .availableProviderTypes()
    .buildRequest()
    .get();

```