---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 24ac3a9f81cd29587ec94f2d4656d31c1451a7c8574c117f1e90010f9e63f07f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57262206"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalConnection externalConnection = new ExternalConnection();
externalConnection.id = "contosohr";
externalConnection.name = "Contoso HR";
externalConnection.description = "Connection to index Contoso HR system";

graphClient.external().connections()
    .buildRequest()
    .post(externalConnection);

```