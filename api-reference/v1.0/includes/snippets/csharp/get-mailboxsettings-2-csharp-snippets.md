---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 05e0d92e030b991810d938cc09073adb62b4be68043d7a453b52a634f95e17f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57373790"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var me = await graphClient.Me
    .Request()
    .Select("MailboxSettings")
    .GetAsync();

var automaticRepliesSetting = me.MailboxSettings.AutomaticRepliesSetting;

```