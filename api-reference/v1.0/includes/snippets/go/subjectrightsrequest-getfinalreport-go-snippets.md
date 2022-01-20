---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 90136dccb9f335216d3db3f2a4c1d07e1904fe68
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131942"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

subjectRightsRequestId := "subjectRightsRequest-id"
result, err := graphClient.Privacy().SubjectRightsRequestsById(&subjectRightsRequestId).GetFinalReport()().Get(nil)


```