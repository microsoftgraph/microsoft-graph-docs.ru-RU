---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c54d89fcd7660d9729fcab4f796cf87848578ccb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337873"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewHistoryDefinitionId := "accessReviewHistoryDefinition-id"
result, err := graphClient.IdentityGovernance().AccessReviews().HistoryDefinitionsById(&accessReviewHistoryDefinitionId).Get(nil)


```