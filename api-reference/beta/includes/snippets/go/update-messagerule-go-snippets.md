---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4629393f537b4c25689c745615c40c158e22e185
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980775"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewMessageRule()
displayName := "Important from partner"
requestBody.SetDisplayName(&displayName)
actions := msgraphsdk.NewMessageRuleActions()
requestBody.SetActions(actions)
markImportance := "high"
actions.SetMarkImportance(&markImportance)
options := &msgraphsdk.MessageRuleRequestBuilderPatchOptions{
    Body: requestBody,
}
mailFolderId := "mailFolder-id"
messageRuleId := "messageRule-id"
graphClient.Me().MailFoldersById(&mailFolderId).MessageRulesById(&messageRuleId).Patch(options)


```