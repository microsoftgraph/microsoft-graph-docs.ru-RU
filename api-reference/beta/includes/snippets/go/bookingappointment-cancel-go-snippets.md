---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aaea46ab976e136e5c3f11dec26b0a031cbfa975
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2022
ms.locfileid: "65341564"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCancellationMessageRequestBody()
cancellationMessage := "Your appointment has been successfully cancelled. Please call us again."
requestBody.SetCancellationMessage(&cancellationMessage)
bookingBusinessId := "bookingBusiness-id"
bookingAppointmentId := "bookingAppointment-id"
graphClient.BookingBusinessesById(&bookingBusinessId).AppointmentsById(&bookingAppointmentId).Cancel(bookingBusiness-id, bookingAppointment-id).Post(requestBody)


```