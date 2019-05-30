---
title: Обновление страницы
description: Обновление содержимого страницы OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 94c3b243dc48b20a3db075835597319e74b26b10
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537318"
---
# <a name="update-page"></a><span data-ttu-id="18e84-103">Обновление страницы</span><span class="sxs-lookup"><span data-stu-id="18e84-103">Update page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18e84-104">Обновление содержимого страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="18e84-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="18e84-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18e84-105">Permissions</span></span>
<span data-ttu-id="18e84-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18e84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18e84-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18e84-108">Permission type</span></span>      | <span data-ttu-id="18e84-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18e84-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18e84-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18e84-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18e84-111">Notes. ReadWrite, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="18e84-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="18e84-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18e84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18e84-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18e84-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="18e84-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18e84-114">Application</span></span> | <span data-ttu-id="18e84-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18e84-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18e84-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18e84-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="18e84-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18e84-117">Request headers</span></span>
| <span data-ttu-id="18e84-118">Имя</span><span class="sxs-lookup"><span data-stu-id="18e84-118">Name</span></span>       | <span data-ttu-id="18e84-119">Тип</span><span class="sxs-lookup"><span data-stu-id="18e84-119">Type</span></span> | <span data-ttu-id="18e84-120">Описание</span><span class="sxs-lookup"><span data-stu-id="18e84-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="18e84-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="18e84-121">Authorization</span></span>  | <span data-ttu-id="18e84-122">string</span><span class="sxs-lookup"><span data-stu-id="18e84-122">string</span></span>  | <span data-ttu-id="18e84-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18e84-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18e84-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18e84-125">Content-Type</span></span> | <span data-ttu-id="18e84-126">string</span><span class="sxs-lookup"><span data-stu-id="18e84-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="18e84-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18e84-127">Request body</span></span>
<span data-ttu-id="18e84-128">В теле запроса добавьте массив объектов [патчконтенткомманд](../resources/patchcontentcommand.md) , которые представляют изменения на странице.</span><span class="sxs-lookup"><span data-stu-id="18e84-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="18e84-129">Дополнительные сведения и примеры приведены в [статье обновление содержимого страницы OneNote](/graph/onenote-update-page).</span><span class="sxs-lookup"><span data-stu-id="18e84-129">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="18e84-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="18e84-130">Response</span></span>

<span data-ttu-id="18e84-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="18e84-131">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="18e84-132">Данные JSON не возвращаются по PATCH-запросу.</span><span class="sxs-lookup"><span data-stu-id="18e84-132">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="18e84-133">Пример</span><span class="sxs-lookup"><span data-stu-id="18e84-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="18e84-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="18e84-134">Request</span></span>
<span data-ttu-id="18e84-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18e84-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="18e84-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="18e84-136">Response</span></span>
<span data-ttu-id="18e84-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="18e84-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenotePage"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="18e84-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="18e84-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="18e84-139">C#</span><span class="sxs-lookup"><span data-stu-id="18e84-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_page-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="18e84-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="18e84-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_page-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/page-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/page-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
