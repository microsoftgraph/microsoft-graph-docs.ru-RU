---
title: Обновление страницы
description: Обновление содержимого OneNote страницы.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 846461d1415d3748059a0c93fe5dc0866dccdc4e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788061"
---
# <a name="update-page"></a><span data-ttu-id="49916-103">Обновление страницы</span><span class="sxs-lookup"><span data-stu-id="49916-103">Update page</span></span>

<span data-ttu-id="49916-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49916-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49916-105">Обновление содержимого OneNote страницы.</span><span class="sxs-lookup"><span data-stu-id="49916-105">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="49916-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49916-106">Permissions</span></span>
<span data-ttu-id="49916-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49916-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49916-109">Permission type</span></span>      | <span data-ttu-id="49916-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49916-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49916-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49916-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49916-112">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49916-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="49916-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49916-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49916-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="49916-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="49916-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49916-115">Application</span></span> | <span data-ttu-id="49916-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49916-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49916-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49916-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="49916-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="49916-118">Request headers</span></span>
| <span data-ttu-id="49916-119">Имя</span><span class="sxs-lookup"><span data-stu-id="49916-119">Name</span></span>       | <span data-ttu-id="49916-120">Тип</span><span class="sxs-lookup"><span data-stu-id="49916-120">Type</span></span> | <span data-ttu-id="49916-121">Описание</span><span class="sxs-lookup"><span data-stu-id="49916-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="49916-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49916-122">Authorization</span></span>  | <span data-ttu-id="49916-123">string</span><span class="sxs-lookup"><span data-stu-id="49916-123">string</span></span>  | <span data-ttu-id="49916-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="49916-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="49916-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="49916-126">Content-Type</span></span> | <span data-ttu-id="49916-127">string</span><span class="sxs-lookup"><span data-stu-id="49916-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="49916-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="49916-128">Request body</span></span>
<span data-ttu-id="49916-129">В теле запроса поставляем массив объектов [patchContentCommand,](../resources/patchcontentcommand.md) которые представляют изменения на странице.</span><span class="sxs-lookup"><span data-stu-id="49916-129">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="49916-130">Дополнительные сведения и примеры см. на <a href="/graph/onenote-update-page">странице Update OneNote.</a></span><span class="sxs-lookup"><span data-stu-id="49916-130">For more information and examples, see <a href="/graph/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="49916-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="49916-131">Response</span></span>

<span data-ttu-id="49916-132">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="49916-132">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="49916-133">Данные JSON не возвращаются по PATCH-запросу.</span><span class="sxs-lookup"><span data-stu-id="49916-133">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="49916-134">Пример</span><span class="sxs-lookup"><span data-stu-id="49916-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49916-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="49916-135">Request</span></span>
<span data-ttu-id="49916-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="49916-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49916-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="49916-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_page"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content
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
# <a name="c"></a>[<span data-ttu-id="49916-138">C#</span><span class="sxs-lookup"><span data-stu-id="49916-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49916-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49916-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49916-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49916-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49916-141">Java</span><span class="sxs-lookup"><span data-stu-id="49916-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="49916-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="49916-142">Response</span></span>
<span data-ttu-id="49916-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="49916-143">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
