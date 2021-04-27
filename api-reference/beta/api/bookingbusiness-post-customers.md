---
title: Создание bookingCustomer
description: Создайте новый объект bookingCustomer.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 5206c6969f2a0f9504cfecd347e7e215577caae1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047870"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="3bf04-103">Создание bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="3bf04-103">Create bookingCustomer</span></span>

<span data-ttu-id="3bf04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bf04-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bf04-105">Создайте новый [объект bookingCustomer.](../resources/bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="3bf04-105">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3bf04-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3bf04-106">Permissions</span></span>
<span data-ttu-id="3bf04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bf04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bf04-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bf04-109">Permission type</span></span>      | <span data-ttu-id="3bf04-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bf04-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bf04-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bf04-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="3bf04-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3bf04-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3bf04-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bf04-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bf04-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bf04-114">Not supported.</span></span>   |
|<span data-ttu-id="3bf04-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bf04-115">Application</span></span> | <span data-ttu-id="3bf04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bf04-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3bf04-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bf04-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="3bf04-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bf04-118">Request headers</span></span>
| <span data-ttu-id="3bf04-119">Имя</span><span class="sxs-lookup"><span data-stu-id="3bf04-119">Name</span></span>       | <span data-ttu-id="3bf04-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3bf04-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3bf04-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3bf04-121">Authorization</span></span>  | <span data-ttu-id="3bf04-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3bf04-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bf04-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3bf04-123">Request body</span></span>
<span data-ttu-id="3bf04-124">В теле запроса указать JSON-представление [объекта bookingCustomer.](../resources/bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="3bf04-124">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="3bf04-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bf04-125">Response</span></span>
<span data-ttu-id="3bf04-126">В случае успеха этот метод возвращает код отклика и `201, Created` [объект bookingCustomer](../resources/bookingcustomer.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="3bf04-126">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bf04-127">Пример</span><span class="sxs-lookup"><span data-stu-id="3bf04-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3bf04-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bf04-128">Request</span></span>
<span data-ttu-id="3bf04-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bf04-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3bf04-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bf04-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3bf04-131">C#</span><span class="sxs-lookup"><span data-stu-id="3bf04-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingcustomer-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3bf04-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bf04-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingcustomer-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3bf04-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bf04-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingcustomer-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3bf04-134">Java</span><span class="sxs-lookup"><span data-stu-id="3bf04-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingcustomer-from-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3bf04-135">В теле запроса указать JSON-представление [объекта bookingCustomer.](../resources/bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="3bf04-135">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3bf04-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3bf04-136">Response</span></span>
<span data-ttu-id="3bf04-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3bf04-137">The following is an example of the response.</span></span> <span data-ttu-id="3bf04-138">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3bf04-138">Note: The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->


