---
title: Список Стаффмемберс
description: Получение списка объектов Букингстаффмембер в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 4d8cfcfcab5478149404f4ac990ab45aa0d61c1c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461766"
---
# <a name="list-staffmembers"></a><span data-ttu-id="67773-103">Список Стаффмемберс</span><span class="sxs-lookup"><span data-stu-id="67773-103">List staffMembers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67773-104">Получение списка объектов [букингстаффмембер](../resources/bookingstaffmember.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="67773-104">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="67773-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67773-105">Permissions</span></span>
<span data-ttu-id="67773-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67773-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67773-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67773-108">Permission type</span></span>      | <span data-ttu-id="67773-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67773-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67773-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67773-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="67773-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="67773-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="67773-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67773-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67773-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67773-113">Not supported.</span></span>   |
|<span data-ttu-id="67773-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67773-114">Application</span></span> | <span data-ttu-id="67773-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67773-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="67773-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67773-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67773-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="67773-117">Optional query parameters</span></span>
<span data-ttu-id="67773-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="67773-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67773-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67773-119">Request headers</span></span>
| <span data-ttu-id="67773-120">Имя</span><span class="sxs-lookup"><span data-stu-id="67773-120">Name</span></span>      |<span data-ttu-id="67773-121">Описание</span><span class="sxs-lookup"><span data-stu-id="67773-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="67773-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67773-122">Authorization</span></span>  | <span data-ttu-id="67773-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="67773-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="67773-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67773-124">Request body</span></span>
<span data-ttu-id="67773-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67773-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="67773-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="67773-126">Response</span></span>
<span data-ttu-id="67773-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [букингстаффмембер](../resources/bookingstaffmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="67773-127">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67773-128">Пример</span><span class="sxs-lookup"><span data-stu-id="67773-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67773-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="67773-129">Request</span></span>
<span data-ttu-id="67773-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67773-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
##### <a name="response"></a><span data-ttu-id="67773-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="67773-131">Response</span></span>
<span data-ttu-id="67773-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="67773-132">The following is an example of the response.</span></span> <span data-ttu-id="67773-133">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="67773-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="67773-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67773-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers",
    "value":[
        {
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
        },
        {
            "id":"71d64d0e-7225-49b6-b0b1-070d476cda51",
            "displayName":"Samantha Booth",
            "emailAddress":"samanthab@M365B489948.OnMicrosoft.com",
            "availabilityIsAffectedByPersonalCalendar":true,
            "colorIndex":0,
            "role":"administrator",
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
                },
                {
                    "day":"saturday",
                    "timeSlots":[

                    ]
                },
                {
                    "day":"sunday",
                    "timeSlots":[

                    ]
                }
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List staffMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list-staffmembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
