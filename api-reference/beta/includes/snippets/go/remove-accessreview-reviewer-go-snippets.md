---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 18f62aa40e3559323de2cbbd5215946f4f06cccb
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2021
ms.locfileid: "61294603"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewId := "accessReview-id"
accessReviewReviewerId := "accessReviewReviewer-id"
graphClient.AccessReviewsById(&accessReviewId).ReviewersById(&accessReviewReviewerId).Delete(nil)


```