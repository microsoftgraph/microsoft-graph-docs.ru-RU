---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5909fb8b3d6c7b2e107549c919413a57dbe08fa6e703f7d8f6080dd7be2b30b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57254529"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcProvisioningPolicy cloudPcProvisioningPolicy = graphClient.deviceManagement().virtualEndpoint().provisioningPolicies("{id}")
    .buildRequest()
    .get();

```