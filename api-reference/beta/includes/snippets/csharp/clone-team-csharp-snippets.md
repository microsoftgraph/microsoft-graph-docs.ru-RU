---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8e33470c7d6132d52b66402603e605f9ad1cee1c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799290"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var displayName = "Library Assist";

var description = "Self help community for library";

var mailNickname = "libassist";

var partsToClone = ClonableTeamParts.Apps | ClonableTeamParts.Tabs | ClonableTeamParts.Settings | ClonableTeamParts.Channels | ClonableTeamParts.Members;

var visibility = TeamVisibilityType.Public;

await graphClient.Teams["{team-id}"]
    .Clone(visibility,partsToClone,displayName,description,mailNickname,null)
    .Request()
    .PostAsync();

```