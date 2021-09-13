---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7a643c2ee88662ed14a36e5945d06d4d6ebb9b7fa620ac35b307bb1b1de386ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57373874"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").homeRealmDiscoveryPolicies("{id}").reference()
    .buildRequest()
    .delete();

```