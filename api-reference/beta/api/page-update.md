---
title: Обновление страницы
description: Обновление содержимого страницы OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 91be57e33bba2d90725beaee8607fd3e2eddb84a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960696"
---
# <a name="update-page"></a><span data-ttu-id="6deae-103">Обновление страницы</span><span class="sxs-lookup"><span data-stu-id="6deae-103">Update page</span></span>

> <span data-ttu-id="6deae-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6deae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6deae-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6deae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6deae-106">Обновление содержимого страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="6deae-106">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="6deae-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6deae-107">Permissions</span></span>
<span data-ttu-id="6deae-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6deae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6deae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6deae-110">Permission type</span></span>      | <span data-ttu-id="6deae-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6deae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6deae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6deae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6deae-113">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6deae-113">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6deae-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6deae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6deae-115">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6deae-115">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6deae-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6deae-116">Application</span></span> | <span data-ttu-id="6deae-117">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6deae-117">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6deae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6deae-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="6deae-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6deae-119">Request headers</span></span>
| <span data-ttu-id="6deae-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6deae-120">Name</span></span>       | <span data-ttu-id="6deae-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6deae-121">Type</span></span> | <span data-ttu-id="6deae-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6deae-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6deae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6deae-123">Authorization</span></span>  | <span data-ttu-id="6deae-124">строка</span><span class="sxs-lookup"><span data-stu-id="6deae-124">string</span></span>  | <span data-ttu-id="6deae-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6deae-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6deae-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6deae-127">Content-Type</span></span> | <span data-ttu-id="6deae-128">строка</span><span class="sxs-lookup"><span data-stu-id="6deae-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="6deae-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6deae-129">Request body</span></span>
<span data-ttu-id="6deae-130">В тексте запроса задаете массив объектов [patchContentCommand](../resources/patchcontentcommand.md) , которые представляют изменения на страницу.</span><span class="sxs-lookup"><span data-stu-id="6deae-130">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page.</span></span> <span data-ttu-id="6deae-131">Дополнительные сведения и примеры в разделе [содержимого страницы OneNote обновления](/graph/onenote-update-page).</span><span class="sxs-lookup"><span data-stu-id="6deae-131">For more information and examples, see [Update OneNote page content](/graph/onenote-update-page).</span></span>

## <a name="response"></a><span data-ttu-id="6deae-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6deae-132">Response</span></span>

<span data-ttu-id="6deae-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`.  Для запроса PATCH не возвращается никаких данных JSON.</span><span class="sxs-lookup"><span data-stu-id="6deae-p105">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="6deae-135">Пример</span><span class="sxs-lookup"><span data-stu-id="6deae-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6deae-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="6deae-136">Request</span></span>
<span data-ttu-id="6deae-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6deae-137">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6deae-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="6deae-138">Response</span></span>
<span data-ttu-id="6deae-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6deae-139">Here is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Update page",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
