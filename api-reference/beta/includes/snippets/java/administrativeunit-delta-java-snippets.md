---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ae68aaa68a267c6597e4cc337382f616998f0ade9d92b0931485027ad68d54c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050910"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnitDeltaCollectionPage delta = graphClient.administrativeUnits()
    .delta()
    .buildRequest()
    .get();

```