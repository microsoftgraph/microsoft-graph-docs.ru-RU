---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c87925b8cf55a05ed9d84a44f155cc138926a193
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799008"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = new BookingStaffMember
{
    WorkingHours = new List<BookingWorkHours>()
    {
        new BookingWorkHours
        {
            Day = DayOfWeek.Monday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"day@odata.type", "#microsoft.graph.dayOfWeek"},
                {"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"}
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Tuesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = new TimeOfDay(17, 0, 0),
                    Start = new TimeOfDay(8, 0, 0)
                }
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"day@odata.type", "#microsoft.graph.dayOfWeek"},
                {"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"}
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Wednesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = new TimeOfDay(17, 0, 0),
                    Start = new TimeOfDay(8, 0, 0)
                }
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"day@odata.type", "#microsoft.graph.dayOfWeek"},
                {"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"}
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Thursday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = new TimeOfDay(17, 0, 0),
                    Start = new TimeOfDay(8, 0, 0)
                }
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"day@odata.type", "#microsoft.graph.dayOfWeek"},
                {"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"}
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Friday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = new TimeOfDay(17, 0, 0),
                    Start = new TimeOfDay(8, 0, 0)
                }
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"day@odata.type", "#microsoft.graph.dayOfWeek"},
                {"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"}
            }
        }
    }
};

await graphClient.BookingBusinesses["{bookingBusiness-id}"].StaffMembers["{bookingStaffMember-id}"]
    .Request()
    .UpdateAsync(bookingStaffMember);

```