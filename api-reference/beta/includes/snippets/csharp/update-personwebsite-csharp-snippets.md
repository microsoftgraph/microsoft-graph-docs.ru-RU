---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 988331405c1e684f67ecec2a22231fcf52c6e04135b1a8e3a2cb137504ffa8e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57193350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personWebsite = new PersonWebsite
{
    Description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
};

await graphClient.Me.Profile.Websites["{personWebsite-id}"]
    .Request()
    .UpdateAsync(personWebsite);

```