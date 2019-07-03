---
title: Обновление страницы
description: Обновление содержимого страницы OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 498288afbe087be9d1bee3f665e74572efee0692
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453931"
---
# <a name="update-page"></a><span data-ttu-id="b02e9-103">Обновление страницы</span><span class="sxs-lookup"><span data-stu-id="b02e9-103">Update page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b02e9-104">Обновление содержимого страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="b02e9-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="b02e9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b02e9-105">Permissions</span></span>
<span data-ttu-id="b02e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b02e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b02e9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b02e9-108">Permission type</span></span>      | <span data-ttu-id="b02e9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b02e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b02e9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b02e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b02e9-111">Notes. ReadWrite, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b02e9-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="b02e9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b02e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b02e9-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b02e9-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="b02e9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b02e9-114">Application</span></span> | <span data-ttu-id="b02e9-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b02e9-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b02e9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b02e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="b02e9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b02e9-117">Request headers</span></span>
| <span data-ttu-id="b02e9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b02e9-118">Name</span></span>       | <span data-ttu-id="b02e9-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b02e9-119">Type</span></span> | <span data-ttu-id="b02e9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b02e9-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b02e9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b02e9-121">Authorization</span></span>  | <span data-ttu-id="b02e9-122">string</span><span class="sxs-lookup"><span data-stu-id="b02e9-122">string</span></span>  | <span data-ttu-id="b02e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b02e9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b02e9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b02e9-125">Content-Type</span></span> | <span data-ttu-id="b02e9-126">string</span><span class="sxs-lookup"><span data-stu-id="b02e9-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="b02e9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b02e9-127">Request body</span></span>
<span data-ttu-id="b02e9-128">В теле запроса добавьте массив объектов [патчконтенткомманд](../resources/patchcontentcommand.md) , которые представляют изменения на странице.</span><span class="sxs-lookup"><span data-stu-id="b02e9-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="b02e9-129">Дополнительные сведения и примеры приведены в [статье обновление содержимого страницы OneNote](/graph/onenote-update-page).</span><span class="sxs-lookup"><span data-stu-id="b02e9-129">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="b02e9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b02e9-130">Response</span></span>

<span data-ttu-id="b02e9-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b02e9-131">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="b02e9-132">Данные JSON не возвращаются по PATCH-запросу.</span><span class="sxs-lookup"><span data-stu-id="b02e9-132">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="b02e9-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b02e9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b02e9-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b02e9-134">Request</span></span>
<span data-ttu-id="b02e9-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b02e9-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b02e9-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="b02e9-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/onenote/pages/{id}/content
Content-type: application/json
Content-length: 312

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-url-or-part-name" alt="image-alt-text" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>new-page-content</li>'
  }
]
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b02e9-137">C#</span><span class="sxs-lookup"><span data-stu-id="b02e9-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b02e9-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="b02e9-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b02e9-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b02e9-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b02e9-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="b02e9-140">Response</span></span>
<span data-ttu-id="b02e9-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b02e9-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
