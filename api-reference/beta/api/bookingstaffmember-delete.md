---
title: Удаление Букингстаффмембер
description: Удаление сотрудника в заданном букингбусинесс.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: f886f3a184599a93ae81135deaf31d37cdd5f4e4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960355"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="db634-103">Удаление Букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="db634-103">Delete bookingStaffMember</span></span>

<span data-ttu-id="db634-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db634-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db634-105">Удаление [сотрудника](../resources/bookingstaffmember.md) в заданном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="db634-105">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="db634-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db634-106">Permissions</span></span>
<span data-ttu-id="db634-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db634-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db634-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db634-109">Permission type</span></span>      | <span data-ttu-id="db634-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db634-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db634-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db634-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="db634-112">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="db634-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="db634-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db634-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db634-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db634-114">Not supported.</span></span>   |
|<span data-ttu-id="db634-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db634-115">Application</span></span> | <span data-ttu-id="db634-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db634-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="db634-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db634-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="db634-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db634-118">Request headers</span></span>
| <span data-ttu-id="db634-119">Имя</span><span class="sxs-lookup"><span data-stu-id="db634-119">Name</span></span>       | <span data-ttu-id="db634-120">Описание</span><span class="sxs-lookup"><span data-stu-id="db634-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db634-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db634-121">Authorization</span></span>  | <span data-ttu-id="db634-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="db634-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="db634-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db634-123">Request body</span></span>
<span data-ttu-id="db634-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db634-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="db634-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="db634-125">Response</span></span>
<span data-ttu-id="db634-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="db634-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db634-128">Пример</span><span class="sxs-lookup"><span data-stu-id="db634-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db634-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="db634-129">Request</span></span>
<span data-ttu-id="db634-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db634-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db634-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="db634-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
# <a name="c"></a>[<span data-ttu-id="db634-132">C#</span><span class="sxs-lookup"><span data-stu-id="db634-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db634-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db634-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db634-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db634-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db634-135">Java</span><span class="sxs-lookup"><span data-stu-id="db634-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingstaffmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="db634-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="db634-136">Response</span></span>
<span data-ttu-id="db634-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="db634-137">The following is an example of the response.</span></span>
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


