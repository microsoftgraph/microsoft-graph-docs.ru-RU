---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 73e84873b25b7e66b32e66e3bb2e2613c449e139
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44219301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Schedule.OpenShifts["OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8"]
    .Request()
    .DeleteAsync();

```