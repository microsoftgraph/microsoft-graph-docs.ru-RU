---
title: Создание bookingStaffMember
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 01983d5a0831b47c2eddfa45dad917f30bdd7b8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076699"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="4843c-104">Создание bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="4843c-104">Create bookingStaffMember</span></span>

 > <span data-ttu-id="4843c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4843c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4843c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4843c-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="4843c-107">Создайте новый [Сотрудник](../resources/bookingstaffmember.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="4843c-107">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="4843c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4843c-108">Permissions</span></span>
<span data-ttu-id="4843c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4843c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4843c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4843c-111">Permission type</span></span>      | <span data-ttu-id="4843c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4843c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4843c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4843c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="4843c-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="4843c-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4843c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4843c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4843c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4843c-116">Not supported.</span></span>   |
|<span data-ttu-id="4843c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4843c-117">Application</span></span> | <span data-ttu-id="4843c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4843c-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4843c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4843c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="4843c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4843c-120">Request headers</span></span>
| <span data-ttu-id="4843c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="4843c-121">Name</span></span>       | <span data-ttu-id="4843c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="4843c-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4843c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4843c-123">Authorization</span></span>  | <span data-ttu-id="4843c-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4843c-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4843c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4843c-125">Request body</span></span>
<span data-ttu-id="4843c-126">В тексте запроса укажите представление JSON объекта [bookingStaffMember](../resources/bookingstaffmember.md) .</span><span class="sxs-lookup"><span data-stu-id="4843c-126">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="4843c-127">Необходимо включить следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="4843c-127">You must include the following properties:</span></span>

- <span data-ttu-id="4843c-128">**displayName**</span><span class="sxs-lookup"><span data-stu-id="4843c-128">**displayName**</span></span>
- <span data-ttu-id="4843c-129">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="4843c-129">**emailAddress**</span></span>
- <span data-ttu-id="4843c-130">**роль**</span><span class="sxs-lookup"><span data-stu-id="4843c-130">**role**</span></span>


## <a name="response"></a><span data-ttu-id="4843c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="4843c-131">Response</span></span>
<span data-ttu-id="4843c-132">Успешно завершена, этот метод возвращает `201, Created` объект [bookingStaffMember](../resources/bookingstaffmember.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="4843c-132">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4843c-133">Пример</span><span class="sxs-lookup"><span data-stu-id="4843c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4843c-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="4843c-134">Request</span></span>
<span data-ttu-id="4843c-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4843c-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingstaffmember_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Content-type: application/json
Content-length: 309

{
    "@odata.type":"#microsoft.graph.bookingStaffMember",
    "colorIndex":1,
    "displayName":"Dana Swope",
    "emailAddress":"danas@contoso.com",
    "role@odata.type":"#microsoft.graph.bookingStaffRole",
    "role":"externalGuest",
    "useBusinessHours":true,
    "workingHours@odata.type":"#Collection(microsoft.graph.bookingWorkHours)",
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"tuesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"wednesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"thursday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"friday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```
<span data-ttu-id="4843c-136">В тексте запроса укажите представление JSON объекта [bookingStaffMember](../resources/bookingstaffmember.md) .</span><span class="sxs-lookup"><span data-stu-id="4843c-136">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4843c-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="4843c-137">Response</span></span>
<span data-ttu-id="4843c-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4843c-138">The following is an example of the response.</span></span> <span data-ttu-id="4843c-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="4843c-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4843c-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4843c-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers/$entity",
    "id":"8ee1c803-a1fa-406d-8259-7ab53233f148",
    "displayName":"Dana Swope",
    "emailAddress":"danas@contoso.com",
    "availabilityIsAffectedByPersonalCalendar":false,
    "colorIndex":1,
    "role":"externalGuest",
    "useBusinessHours":true,
    "workingHours":[
        {
            "day":"monday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"tuesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"wednesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"thursday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"friday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->