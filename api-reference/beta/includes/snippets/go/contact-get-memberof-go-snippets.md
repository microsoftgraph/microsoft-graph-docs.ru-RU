---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a102642bcaf9bfc3e083dcf0362c1ac3bd2c587d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083225"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

orgContactId := "orgContact-id"
result, err := graphClient.ContactsById(&orgContactId).MemberOf().Get(options)


```