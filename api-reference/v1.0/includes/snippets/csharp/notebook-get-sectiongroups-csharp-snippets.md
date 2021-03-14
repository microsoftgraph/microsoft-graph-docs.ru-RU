---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07a8232884e9cc44b8832098aa61d5fc6aa4c3ae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804774"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroups = await graphClient.Me.Onenote.Notebooks["{notebook-id}"].SectionGroups
    .Request()
    .GetAsync();

```