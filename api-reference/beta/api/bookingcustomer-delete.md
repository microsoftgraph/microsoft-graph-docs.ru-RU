---
title: Удаление Букингкустомер
description: Удаление указанного объекта Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 643f70e6e5ba70d7df2518ec487330924d43eeb8
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636032"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="cef46-103">Удаление Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="cef46-103">Delete bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cef46-104">Удаление указанного объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="cef46-104">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cef46-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cef46-105">Permissions</span></span>
<span data-ttu-id="cef46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cef46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cef46-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cef46-108">Permission type</span></span>      | <span data-ttu-id="cef46-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cef46-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cef46-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cef46-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cef46-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="cef46-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="cef46-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cef46-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cef46-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cef46-113">Not supported.</span></span>   |
|<span data-ttu-id="cef46-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cef46-114">Application</span></span> | <span data-ttu-id="cef46-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cef46-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cef46-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cef46-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="cef46-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cef46-117">Request headers</span></span>
| <span data-ttu-id="cef46-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cef46-118">Name</span></span>       | <span data-ttu-id="cef46-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cef46-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cef46-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cef46-120">Authorization</span></span>  | <span data-ttu-id="cef46-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="cef46-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="cef46-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cef46-122">Request body</span></span>
<span data-ttu-id="cef46-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cef46-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cef46-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="cef46-124">Response</span></span>
<span data-ttu-id="cef46-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cef46-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cef46-127">Пример</span><span class="sxs-lookup"><span data-stu-id="cef46-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cef46-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="cef46-128">Request</span></span>
<span data-ttu-id="cef46-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cef46-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
##### <a name="response"></a><span data-ttu-id="cef46-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="cef46-130">Response</span></span>
<span data-ttu-id="cef46-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cef46-131">The following is an example of the response.</span></span> <span data-ttu-id="cef46-132">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="cef46-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cef46-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cef46-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="cef46-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="cef46-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cef46-135">Языках</span><span class="sxs-lookup"><span data-stu-id="cef46-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_bookingcustomer-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cef46-136">Язык</span><span class="sxs-lookup"><span data-stu-id="cef46-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_bookingcustomer-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/bookingcustomer-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingcustomer-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
