---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8e3dd4a0efa3a8107fbb619ed58e1db4c9717d323e39f19e29b66e7ba9774d29
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57249069"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

HomeRealmDiscoveryPolicy homeRealmDiscoveryPolicy = graphClient.policies().homeRealmDiscoveryPolicies("{id}")
    .buildRequest()
    .get();

```