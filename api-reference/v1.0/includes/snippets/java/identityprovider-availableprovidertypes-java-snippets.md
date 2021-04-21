---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 223272a81f191dbd5a2194cfaec40fa537cd26cc
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920248"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderAvailableProviderTypesCollectionPage availableProviderTypes = graphClient.identityProviders()
    .availableProviderTypes()
    .buildRequest()
    .get();

```