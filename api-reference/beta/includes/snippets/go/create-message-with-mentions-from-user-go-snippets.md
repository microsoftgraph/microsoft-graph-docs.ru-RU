---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fc34a72f5a931deaafaee1090ffe99fa56b034b8
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2022
ms.locfileid: "66099548"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessage()
subject := "Party planning"
requestBody.SetSubject(&subject)
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
name := "Samantha Booth"
    emailAddress.SetName(&name)
address := "samanthab@contoso.onmicrosoft.com"
    emailAddress.SetAddress(&address)
}
requestBody.SetMentions( []Mention {
    msgraphsdk.NewMention(),
mentioned := msgraphsdk.NewEmailAddress()
    SetMentioned(mentioned)
name := "Dana Swope"
    mentioned.SetName(&name)
address := "danas@contoso.onmicrosoft.com"
    mentioned.SetAddress(&address)
}
result, err := graphClient.Me().Messages().Post(requestBody)


```