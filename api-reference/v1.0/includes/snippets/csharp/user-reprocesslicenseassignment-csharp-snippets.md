---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bb8263894ca8f83b5fc29d7b34dcfb11287943c9
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2020
ms.locfileid: "41953653"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["047dd774-f1c4-40f2-82f0-278de79f9b83"]
    .ReprocessLicenseAssignment()
    .Request()
    .PostAsync();

```