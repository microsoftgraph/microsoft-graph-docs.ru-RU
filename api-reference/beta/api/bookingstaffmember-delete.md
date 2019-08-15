---
title: Удаление Букингстаффмембер
description: Удаление сотрудника в заданном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: eb6b696ed722c675de792a5d7a46b44048ba4840
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419344"
---
# <a name="delete-bookingstaffmember"></a><span data-ttu-id="2acd8-103">Удаление Букингстаффмембер</span><span class="sxs-lookup"><span data-stu-id="2acd8-103">Delete bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2acd8-104">Удаление [сотрудника](../resources/bookingstaffmember.md) в заданном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="2acd8-104">Delete a [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2acd8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2acd8-105">Permissions</span></span>
<span data-ttu-id="2acd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2acd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2acd8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2acd8-108">Permission type</span></span>      | <span data-ttu-id="2acd8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2acd8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2acd8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2acd8-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2acd8-111">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="2acd8-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2acd8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2acd8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2acd8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2acd8-113">Not supported.</span></span>   |
|<span data-ttu-id="2acd8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2acd8-114">Application</span></span> | <span data-ttu-id="2acd8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2acd8-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2acd8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2acd8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/staffMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="2acd8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2acd8-117">Request headers</span></span>
| <span data-ttu-id="2acd8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2acd8-118">Name</span></span>       | <span data-ttu-id="2acd8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2acd8-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2acd8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2acd8-120">Authorization</span></span>  | <span data-ttu-id="2acd8-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2acd8-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2acd8-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2acd8-122">Request body</span></span>
<span data-ttu-id="2acd8-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2acd8-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2acd8-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="2acd8-124">Response</span></span>
<span data-ttu-id="2acd8-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2acd8-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2acd8-127">Пример</span><span class="sxs-lookup"><span data-stu-id="2acd8-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2acd8-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="2acd8-128">Request</span></span>
<span data-ttu-id="2acd8-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2acd8-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2acd8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2acd8-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingstaffmember"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/5fae928f-6d2d-417a-ad96-4b0caeb362d6
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2acd8-131">C#</span><span class="sxs-lookup"><span data-stu-id="2acd8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2acd8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2acd8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2acd8-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2acd8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2acd8-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2acd8-134">Response</span></span>
<span data-ttu-id="2acd8-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2acd8-135">The following is an example of the response.</span></span>
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
