---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07fbf981c0df7107a0bbd8dd7d00a91aa0f1097ce9b20a7da8917365d219be0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57251246"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageRule messageRule = new MessageRule();
messageRule.displayName = "Important from partner";
MessageRuleActions actions = new MessageRuleActions();
actions.markImportance = Importance.HIGH;
messageRule.actions = actions;

graphClient.me().mailFolders("inbox").messageRules("AQAAAJ5dZqA=")
    .buildRequest()
    .patch(messageRule);

```