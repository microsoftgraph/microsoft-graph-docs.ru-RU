---
title: Получение Букингкустомер
description: Получение свойств и связей объекта Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3d6b51dc43d5f713dbdb99733cf05ca66c1e31f0
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636025"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="902f1-103">Получение Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="902f1-103">Get bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="902f1-104">Получение свойств и связей объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="902f1-104">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="902f1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="902f1-105">Permissions</span></span>
<span data-ttu-id="902f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="902f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="902f1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="902f1-108">Permission type</span></span>      | <span data-ttu-id="902f1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="902f1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="902f1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="902f1-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="902f1-111">Резервирования. Read. ALL, Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="902f1-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="902f1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="902f1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="902f1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="902f1-113">Not supported.</span></span>   |
|<span data-ttu-id="902f1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="902f1-114">Application</span></span> | <span data-ttu-id="902f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="902f1-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="902f1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="902f1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="902f1-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="902f1-117">Optional query parameters</span></span>
<span data-ttu-id="902f1-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="902f1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="902f1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="902f1-119">Request headers</span></span>
| <span data-ttu-id="902f1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="902f1-120">Name</span></span>      |<span data-ttu-id="902f1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="902f1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="902f1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="902f1-122">Authorization</span></span>  | <span data-ttu-id="902f1-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="902f1-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="902f1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="902f1-124">Request body</span></span>
<span data-ttu-id="902f1-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="902f1-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="902f1-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="902f1-126">Response</span></span>
<span data-ttu-id="902f1-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [букингкустомер](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="902f1-127">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="902f1-128">Пример</span><span class="sxs-lookup"><span data-stu-id="902f1-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="902f1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="902f1-129">Request</span></span>
<span data-ttu-id="902f1-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="902f1-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
##### <a name="response"></a><span data-ttu-id="902f1-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="902f1-131">Response</span></span>
<span data-ttu-id="902f1-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="902f1-132">The following is an example of the response.</span></span> <span data-ttu-id="902f1-133">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="902f1-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="902f1-134">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="902f1-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele Vance",
    "emailAddress": "adelev@proseware.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="902f1-135">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="902f1-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="902f1-136">Языках</span><span class="sxs-lookup"><span data-stu-id="902f1-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingcustomer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="902f1-137">Язык</span><span class="sxs-lookup"><span data-stu-id="902f1-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingcustomer-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcustomer-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingcustomer-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
