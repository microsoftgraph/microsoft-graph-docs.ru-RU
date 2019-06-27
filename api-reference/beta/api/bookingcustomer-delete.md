---
title: Удаление Букингкустомер
description: Удаление указанного объекта Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 57b81dec910e8db849e20df39fd2011d6d412215
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257955"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="11c66-103">Удаление Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="11c66-103">Delete bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11c66-104">Удаление указанного объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="11c66-104">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="11c66-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11c66-105">Permissions</span></span>
<span data-ttu-id="11c66-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11c66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11c66-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11c66-108">Permission type</span></span>      | <span data-ttu-id="11c66-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11c66-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11c66-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11c66-110">Delegated (work or school account)</span></span> | <span data-ttu-id="11c66-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="11c66-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="11c66-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11c66-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11c66-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11c66-113">Not supported.</span></span>   |
|<span data-ttu-id="11c66-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="11c66-114">Application</span></span> | <span data-ttu-id="11c66-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11c66-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="11c66-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11c66-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="11c66-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11c66-117">Request headers</span></span>
| <span data-ttu-id="11c66-118">Имя</span><span class="sxs-lookup"><span data-stu-id="11c66-118">Name</span></span>       | <span data-ttu-id="11c66-119">Описание</span><span class="sxs-lookup"><span data-stu-id="11c66-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="11c66-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11c66-120">Authorization</span></span>  | <span data-ttu-id="11c66-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="11c66-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="11c66-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11c66-122">Request body</span></span>
<span data-ttu-id="11c66-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11c66-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="11c66-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="11c66-124">Response</span></span>
<span data-ttu-id="11c66-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="11c66-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11c66-127">Пример</span><span class="sxs-lookup"><span data-stu-id="11c66-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11c66-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="11c66-128">Request</span></span>
<span data-ttu-id="11c66-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11c66-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
##### <a name="response"></a><span data-ttu-id="11c66-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="11c66-130">Response</span></span>
<span data-ttu-id="11c66-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="11c66-131">The following is an example of the response.</span></span> <span data-ttu-id="11c66-132">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="11c66-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="11c66-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11c66-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="11c66-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="11c66-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="11c66-135">C#</span><span class="sxs-lookup"><span data-stu-id="11c66-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_bookingcustomer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11c66-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="11c66-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_bookingcustomer-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="11c66-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="11c66-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_bookingcustomer-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcustomer-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingcustomer-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingcustomer-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
