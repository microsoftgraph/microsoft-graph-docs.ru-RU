---
title: Обновление страницы
description: Обновление содержимого OneNote страницы.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: f6f0fb24188beb64502d2ef91c389f66677465fe
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785139"
---
# <a name="update-page"></a><span data-ttu-id="7a43d-103">Обновление страницы</span><span class="sxs-lookup"><span data-stu-id="7a43d-103">Update page</span></span>

<span data-ttu-id="7a43d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a43d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a43d-105">Обновление содержимого OneNote страницы.</span><span class="sxs-lookup"><span data-stu-id="7a43d-105">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a43d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7a43d-106">Permissions</span></span>
<span data-ttu-id="7a43d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a43d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a43d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7a43d-109">Permission type</span></span>      | <span data-ttu-id="7a43d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7a43d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a43d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7a43d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7a43d-112">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a43d-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="7a43d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7a43d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a43d-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a43d-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="7a43d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7a43d-115">Application</span></span> | <span data-ttu-id="7a43d-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a43d-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a43d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7a43d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="7a43d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7a43d-118">Request headers</span></span>
| <span data-ttu-id="7a43d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7a43d-119">Name</span></span>       | <span data-ttu-id="7a43d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7a43d-120">Type</span></span> | <span data-ttu-id="7a43d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7a43d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7a43d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a43d-122">Authorization</span></span>  | <span data-ttu-id="7a43d-123">string</span><span class="sxs-lookup"><span data-stu-id="7a43d-123">string</span></span>  | <span data-ttu-id="7a43d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a43d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7a43d-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a43d-126">Content-Type</span></span> | <span data-ttu-id="7a43d-127">string</span><span class="sxs-lookup"><span data-stu-id="7a43d-127">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="7a43d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7a43d-128">Request body</span></span>
<span data-ttu-id="7a43d-129">В теле запроса поставляем массив объектов [patchContentCommand,](../resources/patchcontentcommand.md) которые представляют изменения на странице.</span><span class="sxs-lookup"><span data-stu-id="7a43d-129">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="7a43d-130">Дополнительные сведения и примеры см. в [OneNote update OneNote.](/graph/onenote-update-page)</span><span class="sxs-lookup"><span data-stu-id="7a43d-130">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="7a43d-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a43d-131">Response</span></span>

<span data-ttu-id="7a43d-132">При успешном выполнении этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7a43d-132">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="7a43d-133">Данные JSON не возвращаются по PATCH-запросу.</span><span class="sxs-lookup"><span data-stu-id="7a43d-133">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="7a43d-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7a43d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a43d-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7a43d-135">Request</span></span>
<span data-ttu-id="7a43d-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7a43d-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7a43d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a43d-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="7a43d-138">C#</span><span class="sxs-lookup"><span data-stu-id="7a43d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a43d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a43d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a43d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a43d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7a43d-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7a43d-141">Response</span></span>
<span data-ttu-id="7a43d-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7a43d-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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


