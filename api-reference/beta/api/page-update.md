---
title: Обновление страницы
description: Обновление содержимого страницы OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: d80aae98828fa2ad07360e3a5b8d660e5d980b35
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539420"
---
# <a name="update-page"></a><span data-ttu-id="ef103-103">Обновление страницы</span><span class="sxs-lookup"><span data-stu-id="ef103-103">Update page</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef103-104">Обновление содержимого страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="ef103-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef103-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef103-105">Permissions</span></span>
<span data-ttu-id="ef103-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef103-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef103-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef103-108">Permission type</span></span>      | <span data-ttu-id="ef103-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef103-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef103-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef103-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ef103-111">Notes. ReadWrite, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ef103-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef103-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef103-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef103-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ef103-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ef103-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ef103-114">Application</span></span> | <span data-ttu-id="ef103-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef103-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef103-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef103-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="ef103-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ef103-117">Request headers</span></span>
| <span data-ttu-id="ef103-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ef103-118">Name</span></span>       | <span data-ttu-id="ef103-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ef103-119">Type</span></span> | <span data-ttu-id="ef103-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ef103-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ef103-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef103-121">Authorization</span></span>  | <span data-ttu-id="ef103-122">string</span><span class="sxs-lookup"><span data-stu-id="ef103-122">string</span></span>  | <span data-ttu-id="ef103-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef103-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ef103-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef103-125">Content-Type</span></span> | <span data-ttu-id="ef103-126">string</span><span class="sxs-lookup"><span data-stu-id="ef103-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ef103-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef103-127">Request body</span></span>
<span data-ttu-id="ef103-128">В теле запроса добавьте массив объектов [патчконтенткомманд](../resources/patchcontentcommand.md) , которые представляют изменения на странице.</span><span class="sxs-lookup"><span data-stu-id="ef103-128">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="ef103-129">Дополнительные сведения и примеры приведены в [статье обновление содержимого страницы OneNote](/graph/onenote-update-page).</span><span class="sxs-lookup"><span data-stu-id="ef103-129">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="ef103-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef103-130">Response</span></span>

<span data-ttu-id="ef103-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ef103-131">If successful, this method returns a `204 No Content` response code.</span></span>  <span data-ttu-id="ef103-132">Данные JSON не возвращаются по PATCH-запросу.</span><span class="sxs-lookup"><span data-stu-id="ef103-132">No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="ef103-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ef103-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef103-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef103-134">Request</span></span>
<span data-ttu-id="ef103-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ef103-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ef103-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ef103-136">Response</span></span>
<span data-ttu-id="ef103-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ef103-137">Here is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/page-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
