---
title: Список клиентов
description: Получите список объектов bookingCustomer.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: ac91295cc6ac0edf96980d20e97153cd7cac0a29
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524942"
---
# <a name="list-customers"></a><span data-ttu-id="090ee-103">Список клиентов</span><span class="sxs-lookup"><span data-stu-id="090ee-103">List customers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="090ee-104">Получите список объектов [bookingCustomer](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="090ee-104">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="090ee-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="090ee-105">Permissions</span></span>
<span data-ttu-id="090ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="090ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="090ee-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="090ee-108">Permission type</span></span>      | <span data-ttu-id="090ee-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="090ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="090ee-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="090ee-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="090ee-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="090ee-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="090ee-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="090ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="090ee-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="090ee-113">Not supported.</span></span>   |
|<span data-ttu-id="090ee-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="090ee-114">Application</span></span> | <span data-ttu-id="090ee-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="090ee-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="090ee-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="090ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="090ee-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="090ee-117">Optional query parameters</span></span>
<span data-ttu-id="090ee-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="090ee-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="090ee-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="090ee-119">Request headers</span></span>
| <span data-ttu-id="090ee-120">Имя</span><span class="sxs-lookup"><span data-stu-id="090ee-120">Name</span></span>      |<span data-ttu-id="090ee-121">Описание</span><span class="sxs-lookup"><span data-stu-id="090ee-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="090ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="090ee-122">Authorization</span></span>  | <span data-ttu-id="090ee-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="090ee-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="090ee-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="090ee-124">Request body</span></span>
<span data-ttu-id="090ee-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="090ee-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="090ee-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="090ee-126">Response</span></span>
<span data-ttu-id="090ee-127">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [bookingCustomer](../resources/bookingcustomer.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="090ee-127">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="090ee-128">Пример</span><span class="sxs-lookup"><span data-stu-id="090ee-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="090ee-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="090ee-129">Request</span></span>
<span data-ttu-id="090ee-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="090ee-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
##### <a name="response"></a><span data-ttu-id="090ee-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="090ee-131">Response</span></span>
<span data-ttu-id="090ee-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="090ee-132">The following is an example of the response.</span></span> <span data-ttu-id="090ee-133">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="090ee-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="090ee-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="090ee-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers",
    "value": [
        {
            "id": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "displayName": "Bob Kelly",
            "emailAddress": "bobk@tailspintoys.com"
        },
        {
            "id": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "displayName": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list-customers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
