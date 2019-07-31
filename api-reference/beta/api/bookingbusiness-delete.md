---
title: Удаление Букингбусинесс
description: Удаление объекта Букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b4def2ea77facec964ad4960e2c78aac2cb89d8c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945208"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="2ea4e-103">Удаление Букингбусинесс</span><span class="sxs-lookup"><span data-stu-id="2ea4e-103">Delete bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ea4e-104">Удаление объекта [букингбусинесс](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="2ea4e-104">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2ea4e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2ea4e-105">Permissions</span></span>
<span data-ttu-id="2ea4e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ea4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ea4e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2ea4e-108">Permission type</span></span>      | <span data-ttu-id="2ea4e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2ea4e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ea4e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2ea4e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2ea4e-111">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="2ea4e-111">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2ea4e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2ea4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ea4e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ea4e-113">Not supported.</span></span>   |
|<span data-ttu-id="2ea4e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2ea4e-114">Application</span></span> | <span data-ttu-id="2ea4e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ea4e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2ea4e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2ea4e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="2ea4e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2ea4e-117">Request headers</span></span>
| <span data-ttu-id="2ea4e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2ea4e-118">Name</span></span>       | <span data-ttu-id="2ea4e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2ea4e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ea4e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2ea4e-120">Authorization</span></span>  | <span data-ttu-id="2ea4e-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2ea4e-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ea4e-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2ea4e-122">Request body</span></span>
<span data-ttu-id="2ea4e-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2ea4e-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="2ea4e-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ea4e-124">Response</span></span>
<span data-ttu-id="2ea4e-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2ea4e-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ea4e-127">Пример</span><span class="sxs-lookup"><span data-stu-id="2ea4e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ea4e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="2ea4e-128">Request</span></span>
<span data-ttu-id="2ea4e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2ea4e-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2ea4e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ea4e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ea4e-131">C#</span><span class="sxs-lookup"><span data-stu-id="2ea4e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ea4e-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="2ea4e-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ea4e-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2ea4e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2ea4e-134">Java</span><span class="sxs-lookup"><span data-stu-id="2ea4e-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2ea4e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="2ea4e-135">Response</span></span>
<span data-ttu-id="2ea4e-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2ea4e-136">The following is an example of the response.</span></span>
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
