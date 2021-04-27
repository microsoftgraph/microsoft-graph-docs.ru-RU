---
title: Создание bookingBusiness
description: Создание нового бизнеса Microsoft Bookings в клиенте.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 251d1b6d5e73b646216bdb152289808e93882d38
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047884"
---
# <a name="create-bookingbusiness"></a><span data-ttu-id="43707-103">Создание bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="43707-103">Create bookingBusiness</span></span>

<span data-ttu-id="43707-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43707-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43707-105">Создание нового бизнеса Microsoft Bookings в клиенте.</span><span class="sxs-lookup"><span data-stu-id="43707-105">Create a new Microsoft Bookings business in a tenant.</span></span>

<span data-ttu-id="43707-106">Это первый шаг в настройке бизнеса Bookings, в котором необходимо указать имя бизнес-отображения.</span><span class="sxs-lookup"><span data-stu-id="43707-106">This is the first step in setting up a Bookings business where you must specify the business display name.</span></span> <span data-ttu-id="43707-107">Вы можете включить другие сведения, такие как бизнес-адрес, адрес веб-сайта [](bookingbusiness-update.md) и политику планирования, или установить эту информацию позже, обновив **bookingBusiness.**</span><span class="sxs-lookup"><span data-stu-id="43707-107">You can include other information such as business address, web site address, and scheduling policy, or set that information later by [updating](bookingbusiness-update.md) the **bookingBusiness**.</span></span>
## <a name="permissions"></a><span data-ttu-id="43707-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43707-108">Permissions</span></span>
<span data-ttu-id="43707-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43707-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43707-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43707-111">Permission type</span></span>      | <span data-ttu-id="43707-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43707-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43707-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43707-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="43707-114">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="43707-114">Bookings.Manage.All</span></span>  |
|<span data-ttu-id="43707-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43707-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43707-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43707-116">Not supported.</span></span>   |
|<span data-ttu-id="43707-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43707-117">Application</span></span> | <span data-ttu-id="43707-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43707-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="43707-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43707-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses

```
## <a name="request-headers"></a><span data-ttu-id="43707-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43707-120">Request headers</span></span>
| <span data-ttu-id="43707-121">Имя</span><span class="sxs-lookup"><span data-stu-id="43707-121">Name</span></span>       | <span data-ttu-id="43707-122">Описание</span><span class="sxs-lookup"><span data-stu-id="43707-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="43707-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43707-123">Authorization</span></span>  | <span data-ttu-id="43707-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="43707-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="43707-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43707-125">Request body</span></span>
<span data-ttu-id="43707-126">В теле запроса указать JSON-представление [объекта bookingBusiness.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="43707-126">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="43707-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="43707-127">Response</span></span>
<span data-ttu-id="43707-128">В случае успешной работы этот метод возвращает код ответа и `201, Created` [объект bookingBusiness](../resources/bookingbusiness.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="43707-128">If successful, this method returns `201, Created` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43707-129">Пример</span><span class="sxs-lookup"><span data-stu-id="43707-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43707-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="43707-130">Request</span></span>
<span data-ttu-id="43707-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43707-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="43707-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="43707-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="43707-133">C#</span><span class="sxs-lookup"><span data-stu-id="43707-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingbusiness-from-bookingbusinesses-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43707-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43707-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingbusiness-from-bookingbusinesses-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43707-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43707-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingbusiness-from-bookingbusinesses-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43707-136">Java</span><span class="sxs-lookup"><span data-stu-id="43707-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingbusiness-from-bookingbusinesses-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="43707-137">В теле запроса указать JSON-представление [объекта bookingBusiness.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="43707-137">In the request body, supply a JSON representation of [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="43707-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="43707-138">Response</span></span>
<span data-ttu-id="43707-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="43707-139">The following is an example of the response.</span></span> <span data-ttu-id="43707-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="43707-140">Note: The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->


