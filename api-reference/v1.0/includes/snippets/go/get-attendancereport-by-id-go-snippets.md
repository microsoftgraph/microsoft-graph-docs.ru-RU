---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d0f82da36103370ed6d560635bc075ee0aa54999
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117258"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MeetingAttendanceReportRequestBuilderGetQueryParameters{
    Expand: "attendanceRecords",
}
options := &msgraphsdk.MeetingAttendanceReportRequestBuilderGetOptions{
    Q: requestParameters,
}
onlineMeetingId := "onlineMeeting-id"
meetingAttendanceReportId := "meetingAttendanceReport-id"
result, err := graphClient.Me().OnlineMeetingsById(&onlineMeetingId).AttendanceReportsById(&meetingAttendanceReportId).Get(options)


```