---
title: Удаление bookingCustomer
description: Удаление указанного объекта bookingCustomer.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 83cdf9e3f3521f85fe0a078951a1e510cb355224
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047835"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="5fe6f-103">Удаление bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="5fe6f-103">Delete bookingCustomer</span></span>

<span data-ttu-id="5fe6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fe6f-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fe6f-105">Удаление указанного [объекта bookingCustomer.](../resources/bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="5fe6f-105">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5fe6f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5fe6f-106">Permissions</span></span>
<span data-ttu-id="5fe6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fe6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fe6f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fe6f-109">Permission type</span></span>      | <span data-ttu-id="5fe6f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fe6f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fe6f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fe6f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5fe6f-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="5fe6f-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5fe6f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fe6f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fe6f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fe6f-114">Not supported.</span></span>   |
|<span data-ttu-id="5fe6f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fe6f-115">Application</span></span> | <span data-ttu-id="5fe6f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fe6f-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5fe6f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fe6f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="5fe6f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fe6f-118">Request headers</span></span>
| <span data-ttu-id="5fe6f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5fe6f-119">Name</span></span>       | <span data-ttu-id="5fe6f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5fe6f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5fe6f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fe6f-121">Authorization</span></span>  | <span data-ttu-id="5fe6f-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5fe6f-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5fe6f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5fe6f-123">Request body</span></span>
<span data-ttu-id="5fe6f-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5fe6f-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="5fe6f-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fe6f-125">Response</span></span>
<span data-ttu-id="5fe6f-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="5fe6f-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5fe6f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="5fe6f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5fe6f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fe6f-129">Request</span></span>
<span data-ttu-id="5fe6f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5fe6f-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5fe6f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fe6f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
# <a name="c"></a>[<span data-ttu-id="5fe6f-132">C#</span><span class="sxs-lookup"><span data-stu-id="5fe6f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fe6f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fe6f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fe6f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fe6f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5fe6f-135">Java</span><span class="sxs-lookup"><span data-stu-id="5fe6f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5fe6f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="5fe6f-136">Response</span></span>
<span data-ttu-id="5fe6f-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5fe6f-137">The following is an example of the response.</span></span> <span data-ttu-id="5fe6f-138">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5fe6f-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->


