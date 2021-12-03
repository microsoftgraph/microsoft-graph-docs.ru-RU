---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3a914cc8ac007acd749afb660180019cdcc2c0a5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61296009"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerRosterId := "plannerRoster-id"
plannerRosterMemberId := "plannerRosterMember-id"
graphClient.Planner().RostersById(&plannerRosterId).MembersById(&plannerRosterMemberId).Delete(nil)


```