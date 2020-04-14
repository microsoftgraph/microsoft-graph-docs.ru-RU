---
title: Удаление Букингбусинесс
description: Удаление объекта Букингбусинесс.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 80935b618ae4a6badadd5eb2bbc49199326c6e6f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43367415"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="9cbd8-103">Удаление Букингбусинесс</span><span class="sxs-lookup"><span data-stu-id="9cbd8-103">Delete bookingBusiness</span></span>

<span data-ttu-id="9cbd8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cbd8-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9cbd8-105">Удаление объекта [букингбусинесс](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="9cbd8-105">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9cbd8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9cbd8-106">Permissions</span></span>
<span data-ttu-id="9cbd8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cbd8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cbd8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9cbd8-109">Permission type</span></span>      | <span data-ttu-id="9cbd8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9cbd8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9cbd8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9cbd8-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="9cbd8-112">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="9cbd8-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9cbd8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9cbd8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9cbd8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cbd8-114">Not supported.</span></span>   |
|<span data-ttu-id="9cbd8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9cbd8-115">Application</span></span> | <span data-ttu-id="9cbd8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9cbd8-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9cbd8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9cbd8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9cbd8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9cbd8-118">Request headers</span></span>
| <span data-ttu-id="9cbd8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9cbd8-119">Name</span></span>       | <span data-ttu-id="9cbd8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9cbd8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9cbd8-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9cbd8-121">Authorization</span></span>  | <span data-ttu-id="9cbd8-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9cbd8-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cbd8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9cbd8-123">Request body</span></span>
<span data-ttu-id="9cbd8-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9cbd8-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9cbd8-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="9cbd8-125">Response</span></span>
<span data-ttu-id="9cbd8-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9cbd8-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cbd8-128">Пример</span><span class="sxs-lookup"><span data-stu-id="9cbd8-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9cbd8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="9cbd8-129">Request</span></span>
<span data-ttu-id="9cbd8-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9cbd8-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9cbd8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="9cbd8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
# <a name="c"></a>[<span data-ttu-id="9cbd8-132">C#</span><span class="sxs-lookup"><span data-stu-id="9cbd8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9cbd8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9cbd8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9cbd8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9cbd8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9cbd8-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="9cbd8-135">Response</span></span>
<span data-ttu-id="9cbd8-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9cbd8-136">The following is an example of the response.</span></span>
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
