---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bdf58c7d8d8dc77de4add86028b0539f6fbce6bb
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2022
ms.locfileid: "62227589"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationUserId := "educationUser-id"
result, err := graphClient.Education().UsersById(&educationUserId).TaughtClasses().Get(nil)


```