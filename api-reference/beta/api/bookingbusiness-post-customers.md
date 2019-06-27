---
title: Создание Букингкустомер
description: Создание нового объекта Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a7ad80e8caf0e8c38479fc58dc7b677c58617770
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258158"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="a12eb-103">Создание Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="a12eb-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a12eb-104">Создание нового объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="a12eb-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a12eb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a12eb-105">Permissions</span></span>
<span data-ttu-id="a12eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a12eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a12eb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a12eb-108">Permission type</span></span>      | <span data-ttu-id="a12eb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a12eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a12eb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a12eb-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a12eb-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="a12eb-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a12eb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a12eb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a12eb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a12eb-113">Not supported.</span></span>   |
|<span data-ttu-id="a12eb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a12eb-114">Application</span></span> | <span data-ttu-id="a12eb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a12eb-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a12eb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a12eb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="a12eb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a12eb-117">Request headers</span></span>
| <span data-ttu-id="a12eb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="a12eb-118">Name</span></span>       | <span data-ttu-id="a12eb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a12eb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a12eb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a12eb-120">Authorization</span></span>  | <span data-ttu-id="a12eb-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a12eb-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a12eb-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a12eb-122">Request body</span></span>
<span data-ttu-id="a12eb-123">В тексте запроса добавьте представление объекта [букингкустомер](../resources/bookingcustomer.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a12eb-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="a12eb-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="a12eb-124">Response</span></span>
<span data-ttu-id="a12eb-125">В случае успешного выполнения этот метод `201, Created` возвращает код отклика и объект [букингкустомер](../resources/bookingcustomer.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a12eb-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a12eb-126">Пример</span><span class="sxs-lookup"><span data-stu-id="a12eb-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a12eb-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="a12eb-127">Request</span></span>
<span data-ttu-id="a12eb-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a12eb-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomer_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
Content-type: application/json

{
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
<span data-ttu-id="a12eb-129">В тексте запроса добавьте представление объекта [букингкустомер](../resources/bookingcustomer.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a12eb-129">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a12eb-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a12eb-130">Response</span></span>
<span data-ttu-id="a12eb-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a12eb-131">The following is an example of the response.</span></span> <span data-ttu-id="a12eb-132">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="a12eb-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a12eb-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a12eb-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "36038f36-634e-44e4-9415-d7d59c2347aa",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a12eb-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a12eb-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a12eb-135">C#</span><span class="sxs-lookup"><span data-stu-id="a12eb-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_bookingcustomer_from_bookingbusiness-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a12eb-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="a12eb-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_bookingcustomer_from_bookingbusiness-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a12eb-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a12eb-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_bookingcustomer_from_bookingbusiness-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
