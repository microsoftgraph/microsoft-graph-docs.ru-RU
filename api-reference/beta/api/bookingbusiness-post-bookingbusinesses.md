---
title: Создание Букингбусинесс
description: Создайте новую бизнес-деятельность Майкрософт в клиенте.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a7818556d687d5e967f704316dd16e9c4eb2c02d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258102"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="0ced6-103">Создание Букингбусинесс</span><span class="sxs-lookup"><span data-stu-id="0ced6-103">Create bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ced6-104">Создайте новую бизнес-деятельность Майкрософт в клиенте.</span><span class="sxs-lookup"><span data-stu-id="0ced6-104">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="0ced6-105">Это первый шаг при настройке учета для бизнеса, в котором необходимо указать отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="0ced6-105">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="0ced6-106">Вы можете включить другие сведения, такие как рабочий адрес, адрес веб-сайта и политика планирования, или задать эту информацию позже [](bookingbusiness-update.md) , обновив **букингбусинесс**.</span><span class="sxs-lookup"><span data-stu-id="0ced6-106">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="0ced6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ced6-107">Permissions</span></span>
<span data-ttu-id="0ced6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ced6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ced6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ced6-110">Permission type</span></span>      | <span data-ttu-id="0ced6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ced6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ced6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ced6-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0ced6-113">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="0ced6-113">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="0ced6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ced6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ced6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ced6-115">Not supported.</span></span>   |
|<span data-ttu-id="0ced6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ced6-116">Application</span></span> | <span data-ttu-id="0ced6-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ced6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ced6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ced6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="0ced6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ced6-119">Request headers</span></span>
| <span data-ttu-id="0ced6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0ced6-120">Name</span></span>       | <span data-ttu-id="0ced6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0ced6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ced6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ced6-122">Authorization</span></span>  | <span data-ttu-id="0ced6-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0ced6-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ced6-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ced6-124">Request body</span></span>
<span data-ttu-id="0ced6-125">В тексте запроса добавьте представление объекта [букингбусинесс](../resources/bookingbusiness.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ced6-125">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="0ced6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ced6-126">Response</span></span>
<span data-ttu-id="0ced6-127">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и объект [букингбусинесс](../resources/bookingbusiness.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ced6-127">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ced6-128">Пример</span><span class="sxs-lookup"><span data-stu-id="0ced6-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ced6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ced6-129">Request</span></span>
<span data-ttu-id="0ced6-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ced6-130">The following is an example of the request.</span></span>
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
<span data-ttu-id="0ced6-131">В тексте запроса добавьте представление объекта [букингбусинесс](../resources/bookingbusiness.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ced6-131">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0ced6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ced6-132">Response</span></span>
<span data-ttu-id="0ced6-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ced6-133">The following is an example of the response.</span></span> <span data-ttu-id="0ced6-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="0ced6-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0ced6-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ced6-135">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0ced6-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="0ced6-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0ced6-137">C#</span><span class="sxs-lookup"><span data-stu-id="0ced6-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_bookingbusiness_from_bookingbusinesses-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0ced6-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="0ced6-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_bookingbusiness_from_bookingbusinesses-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0ced6-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0ced6-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_bookingbusiness_from_bookingbusinesses-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-post-bookingbusinesses.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-post-bookingbusinesses.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-post-bookingbusinesses.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
