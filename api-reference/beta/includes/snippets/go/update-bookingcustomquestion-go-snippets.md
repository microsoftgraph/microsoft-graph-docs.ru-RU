---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07687240e50df5e9471c1f219ae00f8d529b0b15
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094566"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingCustomQuestion()
displayName := "What is your age?"
requestBody.SetDisplayName(&displayName)
answerInputType := "text"
requestBody.SetAnswerInputType(&answerInputType)
requestBody.SetAnswerOptions( []string {
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.bookingCustomQuestion",
}
options := &msgraphsdk.BookingCustomQuestionRequestBuilderPatchOptions{
    Body: requestBody,
}
bookingBusinessId := "bookingBusiness-id"
bookingCustomQuestionId := "bookingCustomQuestion-id"
graphClient.BookingBusinessesById(&bookingBusinessId).CustomQuestionsById(&bookingCustomQuestionId).Patch(options)


```