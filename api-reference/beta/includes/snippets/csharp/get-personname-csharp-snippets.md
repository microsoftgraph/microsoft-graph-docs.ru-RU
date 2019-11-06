---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2c85d09d8f8e9362cf3a9112229a7c976609ee04
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998090"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personName = await graphClient.Me.Profile.Names["{id}"]
    .Request()
    .GetAsync();

```