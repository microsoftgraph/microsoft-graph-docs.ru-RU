---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f3aee042bb90f1ea50a1aa3930e993c2e0bb7f0c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340081"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessageRule()
displayName := "Important from partner"
requestBody.SetDisplayName(&displayName)
actions := msgraphsdk.NewMessageRuleActions()
requestBody.SetActions(actions)
markImportance := "high"
actions.SetMarkImportance(&markImportance)
mailFolderId := "mailFolder-id"
messageRuleId := "messageRule-id"
graphClient.Me().MailFoldersById(&mailFolderId).MessageRulesById(&messageRuleId).Patch(requestBody)


```