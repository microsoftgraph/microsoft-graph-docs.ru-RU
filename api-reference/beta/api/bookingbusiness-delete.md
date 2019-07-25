---
title: Удаление Букингбусинесс
description: Удаление объекта Букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6c5f68ec3df3256f94454ebbe3f0253375e98776
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865808"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="84fa7-103">Удаление Букингбусинесс</span><span class="sxs-lookup"><span data-stu-id="84fa7-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84fa7-104">Удаление объекта [букингбусинесс](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="84fa7-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="84fa7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84fa7-105">Permissions</span></span>
<span data-ttu-id="84fa7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84fa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84fa7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84fa7-108">Permission type</span></span>      | <span data-ttu-id="84fa7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84fa7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84fa7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84fa7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="84fa7-111">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="84fa7-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="84fa7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84fa7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84fa7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84fa7-113">Not supported.</span></span>   |
|<span data-ttu-id="84fa7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84fa7-114">Application</span></span> | <span data-ttu-id="84fa7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84fa7-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="84fa7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84fa7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="84fa7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84fa7-117">Request headers</span></span>
| <span data-ttu-id="84fa7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="84fa7-118">Name</span></span>       | <span data-ttu-id="84fa7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="84fa7-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="84fa7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84fa7-120">Authorization</span></span>  | <span data-ttu-id="84fa7-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="84fa7-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="84fa7-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84fa7-122">Request body</span></span>
<span data-ttu-id="84fa7-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84fa7-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="84fa7-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="84fa7-124">Response</span></span>
<span data-ttu-id="84fa7-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="84fa7-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84fa7-127">Пример</span><span class="sxs-lookup"><span data-stu-id="84fa7-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84fa7-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="84fa7-128">Request</span></span>
<span data-ttu-id="84fa7-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84fa7-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="84fa7-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="84fa7-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="84fa7-131">C#</span><span class="sxs-lookup"><span data-stu-id="84fa7-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84fa7-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="84fa7-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="84fa7-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="84fa7-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="84fa7-134">Java</span><span class="sxs-lookup"><span data-stu-id="84fa7-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="84fa7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="84fa7-135">Response</span></span>
<span data-ttu-id="84fa7-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="84fa7-136">The following is an example of the response.</span></span>
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
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
