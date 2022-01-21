---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3a782e14fefa3ffe4473d766b4826d310ff8674d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098954"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

serviceHealthIssueId := "serviceHealthIssue-id"
result, err := graphClient.Admin().ServiceAnnouncement().IssuesById(&serviceHealthIssueId).IncidentReport()().Get(nil)


```