---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cecba6ba237f2ca0cc1487cb4d8d5d9503f7f884
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975174"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

educationSchoolId := "educationSchool-id"
result, err := graphClient.Education().SchoolsById(&educationSchoolId).AdministrativeUnit().Get(options)


```