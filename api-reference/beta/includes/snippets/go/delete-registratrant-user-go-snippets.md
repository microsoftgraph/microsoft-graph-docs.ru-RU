---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 91947b20205f19f1d7be9b61fd1776b2b1569694
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61294758"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
onlineMeetingId := "onlineMeeting-id"
meetingRegistrantId := "meetingRegistrant-id"
graphClient.UsersById(&userId).OnlineMeetingsById(&onlineMeetingId).Registration().RegistrantsById(&meetingRegistrantId).Delete(nil)


```