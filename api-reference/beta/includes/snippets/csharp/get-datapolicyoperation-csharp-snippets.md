---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 72bb612b54efb0aadbc800c3d8a12ab6fcadbe44b4b4fcfabed95de1ec2fd40c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57199079"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dataPolicyOperation = await graphClient.DataPolicyOperations["{dataPolicyOperation-id}"]
    .Request()
    .GetAsync();

```