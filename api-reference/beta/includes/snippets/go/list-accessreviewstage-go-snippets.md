---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff31eaf102287edf2147e39e65c95cb716317f9c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65340447"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
accessReviewInstanceId := "accessReviewInstance-id"
result, err := graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).InstancesById(&accessReviewInstanceId).Stages().Get()


```