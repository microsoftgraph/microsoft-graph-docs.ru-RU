---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9793ba64e53b5f1305d2c743eacaa3d79c07940c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684509"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Groups
    .Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select("displayName,description,mailNickname")
    .GetAsync();

```