---
title: Создание bookingBusiness
description: Создание нового резервирования Microsoft business в клиент.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 95a9217392953d287689dca7a7b6f4c74fbe6383
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519250"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="d7399-103">Создание bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="d7399-103">Create bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7399-104">Создание нового резервирования Microsoft business в клиент.</span><span class="sxs-lookup"><span data-stu-id="d7399-104">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="d7399-105">Это первый шаг в настройке business резервирования, где необходимо указать отображаемое имя бизнес.</span><span class="sxs-lookup"><span data-stu-id="d7399-105">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="d7399-106">Можно включить другие сведения, такие как рабочий адрес, адрес веб-сайта и планирования политики или задать эти сведения позже, [изменив](bookingbusiness-update.md) **bookingBusiness**.</span><span class="sxs-lookup"><span data-stu-id="d7399-106">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7399-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7399-107">Permissions</span></span>
<span data-ttu-id="d7399-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7399-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7399-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7399-110">Permission type</span></span>      | <span data-ttu-id="d7399-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7399-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7399-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7399-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="d7399-113">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="d7399-113">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="d7399-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7399-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7399-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7399-115">Not supported.</span></span>   |
|<span data-ttu-id="d7399-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7399-116">Application</span></span> | <span data-ttu-id="d7399-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7399-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7399-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7399-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="d7399-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7399-119">Request headers</span></span>
| <span data-ttu-id="d7399-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d7399-120">Name</span></span>       | <span data-ttu-id="d7399-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d7399-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7399-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7399-122">Authorization</span></span>  | <span data-ttu-id="d7399-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d7399-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7399-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7399-124">Request body</span></span>
<span data-ttu-id="d7399-125">В тексте запроса укажите представление JSON объекта [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="d7399-125">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="d7399-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7399-126">Response</span></span>
<span data-ttu-id="d7399-127">Успешно завершена, этот метод возвращает `201, Created` объект [bookingBusiness](../resources/bookingbusiness.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d7399-127">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7399-128">Пример</span><span class="sxs-lookup"><span data-stu-id="d7399-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7399-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7399-129">Request</span></span>
<span data-ttu-id="d7399-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7399-130">The following is an example of the request.</span></span>
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
<span data-ttu-id="d7399-131">В тексте запроса укажите представление JSON объекта [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="d7399-131">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d7399-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7399-132">Response</span></span>
<span data-ttu-id="d7399-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d7399-133">The following is an example of the response.</span></span> <span data-ttu-id="d7399-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="d7399-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d7399-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7399-135">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-bookingbusinesses.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
