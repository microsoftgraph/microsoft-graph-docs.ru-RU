---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f2c44369d1397d46bcd96c565b4f40ca05f285d6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63417100"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

calendarGroupId := "calendarGroup-id"
result, err := graphClient.Me().CalendarGroupsById(&calendarGroupId).Delete(nil)


```