---
title: Удаление Букингстаффмембер
description: Удаление сотрудника в заданном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 42086e0a8623adf717943d84ad92816ea13e917b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441076"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="6f6e0-103">Удаление Букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="6f6e0-103">Delete bookingStaffMember</span></span>

<span data-ttu-id="6f6e0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6f6e0-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f6e0-105">Удаление [сотрудника](../resources/bookingstaffmember.md) в заданном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="6f6e0-105">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="6f6e0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f6e0-106">Permissions</span></span>
<span data-ttu-id="6f6e0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f6e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f6e0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f6e0-109">Permission type</span></span>      | <span data-ttu-id="6f6e0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f6e0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f6e0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f6e0-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="6f6e0-112">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="6f6e0-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6f6e0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f6e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f6e0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f6e0-114">Not supported.</span></span>   |
|<span data-ttu-id="6f6e0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f6e0-115">Application</span></span> | <span data-ttu-id="6f6e0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f6e0-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6f6e0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f6e0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="6f6e0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f6e0-118">Request headers</span></span>
| <span data-ttu-id="6f6e0-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6f6e0-119">Name</span></span>       | <span data-ttu-id="6f6e0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6f6e0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6f6e0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f6e0-121">Authorization</span></span>  | <span data-ttu-id="6f6e0-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6f6e0-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f6e0-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f6e0-123">Request body</span></span>
<span data-ttu-id="6f6e0-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f6e0-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="6f6e0-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f6e0-125">Response</span></span>
<span data-ttu-id="6f6e0-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6f6e0-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f6e0-128">Пример</span><span class="sxs-lookup"><span data-stu-id="6f6e0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f6e0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f6e0-129">Request</span></span>
<span data-ttu-id="6f6e0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f6e0-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6f6e0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6f6e0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
# <a name="c"></a>[<span data-ttu-id="6f6e0-132">C#</span><span class="sxs-lookup"><span data-stu-id="6f6e0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6f6e0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6f6e0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6f6e0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6f6e0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6f6e0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f6e0-135">Response</span></span>
<span data-ttu-id="6f6e0-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6f6e0-136">The following is an example of the response.</span></span>
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
  "description": "Delete bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
