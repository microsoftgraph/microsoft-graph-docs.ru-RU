---
title: Создание bookingBusiness
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: bfecb479a04f991799eb239c643e2cc521d8332c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894476"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="54278-104">Создание bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="54278-104">Create bookingBusiness</span></span>

 > <span data-ttu-id="54278-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54278-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54278-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54278-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="54278-107">Создание нового резервирования Microsoft business в клиент.</span><span class="sxs-lookup"><span data-stu-id="54278-107">Create a new Microsoft Bookings business in a tenant.</span></span> 

<span data-ttu-id="54278-108">Это первый шаг в настройке business резервирования, где необходимо указать отображаемое имя бизнес.</span><span class="sxs-lookup"><span data-stu-id="54278-108">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="54278-109">Можно включить другие сведения, такие как рабочий адрес, адрес веб-сайта и планирования политики или задать эти сведения позже, [изменив](bookingbusiness-update.md) **bookingBusiness**.</span><span class="sxs-lookup"><span data-stu-id="54278-109">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="54278-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54278-110">Permissions</span></span>
<span data-ttu-id="54278-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54278-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54278-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54278-113">Permission type</span></span>      | <span data-ttu-id="54278-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54278-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54278-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54278-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="54278-116">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="54278-116">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="54278-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54278-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54278-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54278-118">Not supported.</span></span>   |
|<span data-ttu-id="54278-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54278-119">Application</span></span> | <span data-ttu-id="54278-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54278-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="54278-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54278-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="54278-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54278-122">Request headers</span></span>
| <span data-ttu-id="54278-123">Имя</span><span class="sxs-lookup"><span data-stu-id="54278-123">Name</span></span>       | <span data-ttu-id="54278-124">Описание</span><span class="sxs-lookup"><span data-stu-id="54278-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="54278-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="54278-125">Authorization</span></span>  | <span data-ttu-id="54278-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="54278-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="54278-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="54278-127">Request body</span></span>
<span data-ttu-id="54278-128">В тексте запроса укажите представление JSON объекта [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="54278-128">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="54278-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="54278-129">Response</span></span>
<span data-ttu-id="54278-130">Успешно завершена, этот метод возвращает `201, Created` объект [bookingBusiness](../resources/bookingbusiness.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="54278-130">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54278-131">Пример</span><span class="sxs-lookup"><span data-stu-id="54278-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54278-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="54278-132">Request</span></span>
<span data-ttu-id="54278-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54278-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingbusiness_from_bookingbusinesses"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Content-type: application/json

{
    "displayName":"Fourth Coffee",
    "address":{
        "type":"mall",
        "postOfficeBox":"P.O. Box 123",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "phone":"206-555-0100",
    "email":"manager@fourthcoffee.com",
    "webSiteUrl":"https://www.fourthcoffee.com",
    "defaultCurrencyIso":"USD"
}
```
<span data-ttu-id="54278-134">В тексте запроса укажите представление JSON объекта [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="54278-134">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="54278-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="54278-135">Response</span></span>
<span data-ttu-id="54278-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54278-136">The following is an example of the response.</span></span> <span data-ttu-id="54278-137">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="54278-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="54278-138">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="54278-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses/$entity",
    "id":"fourthcoffee@M365B489948.onmicrosoft.com",
    "displayName":"Fourth Coffee",
    "businessType":"",
    "phone":"206-555-0100",
    "email":"manager@fourthcoffee.com",
    "webSiteUrl":"https://www.fourthcoffee.com",
    "defaultCurrencyIso":"USD",
    "isPublished":false,
    "publicUrl":null,
    "address":{
        "type":"mall",
        "postOfficeBox":"P.O. Box 123",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "businessHours":[
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
    ],
    "schedulingPolicy":{
        "timeSlotInterval":"PT30M",
        "minimumLeadTime":"P1D",
        "maximumAdvance":"P365D",
        "sendConfirmationsToOwner":true,
        "allowStaffSelection":true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
