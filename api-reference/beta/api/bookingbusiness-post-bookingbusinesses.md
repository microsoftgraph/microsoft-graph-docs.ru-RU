---
title: Создание Букингбусинесс
description: Создайте новую бизнес-деятельность Майкрософт в клиенте.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 53f675eb0b81ca7a63fe38eb08468039fc08f7c5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322612"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="48982-103">Создание Букингбусинесс</span><span class="sxs-lookup"><span data-stu-id="48982-103">Create bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48982-104">Создайте новую бизнес-деятельность Майкрософт в клиенте.</span><span class="sxs-lookup"><span data-stu-id="48982-104">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="48982-105">Это первый шаг при настройке учета для бизнеса, в котором необходимо указать отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="48982-105">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="48982-106">Вы можете включить другие сведения, такие как рабочий адрес, адрес веб-сайта и политика планирования, или задать эту информацию позже [](bookingbusiness-update.md) , обновив **букингбусинесс**.</span><span class="sxs-lookup"><span data-stu-id="48982-106">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="48982-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48982-107">Permissions</span></span>
<span data-ttu-id="48982-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48982-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48982-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48982-110">Permission type</span></span>      | <span data-ttu-id="48982-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48982-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48982-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48982-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="48982-113">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="48982-113">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="48982-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48982-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48982-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48982-115">Not supported.</span></span>   |
|<span data-ttu-id="48982-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48982-116">Application</span></span> | <span data-ttu-id="48982-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48982-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48982-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48982-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="48982-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48982-119">Request headers</span></span>
| <span data-ttu-id="48982-120">Имя</span><span class="sxs-lookup"><span data-stu-id="48982-120">Name</span></span>       | <span data-ttu-id="48982-121">Описание</span><span class="sxs-lookup"><span data-stu-id="48982-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48982-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48982-122">Authorization</span></span>  | <span data-ttu-id="48982-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="48982-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="48982-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="48982-124">Request body</span></span>
<span data-ttu-id="48982-125">В тексте запроса добавьте представление объекта [Букингбусинесс](../resources/bookingbusiness.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48982-125">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="48982-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="48982-126">Response</span></span>
<span data-ttu-id="48982-127">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и объект [букингбусинесс](../resources/bookingbusiness.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48982-127">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48982-128">Пример</span><span class="sxs-lookup"><span data-stu-id="48982-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48982-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="48982-129">Request</span></span>
<span data-ttu-id="48982-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48982-130">The following is an example of the request.</span></span>
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
<span data-ttu-id="48982-131">В тексте запроса добавьте представление объекта [Букингбусинесс](../resources/bookingbusiness.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48982-131">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="48982-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="48982-132">Response</span></span>
<span data-ttu-id="48982-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="48982-133">The following is an example of the response.</span></span> <span data-ttu-id="48982-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="48982-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="48982-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48982-135">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
