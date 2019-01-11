---
title: Обновление страницы
description: Обновление содержимого страницы OneNote.
localization_priority: Normal
ms.openlocfilehash: ee5e55ce206ac1f3069c5629f8c0f674f209363c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850178"
---
# <a name="update-page"></a><span data-ttu-id="ceeb0-103">Обновление страницы</span><span class="sxs-lookup"><span data-stu-id="ceeb0-103">Update page</span></span>

<span data-ttu-id="ceeb0-104">Обновление содержимого страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="ceeb0-104">Update the content of a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="ceeb0-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ceeb0-105">Permissions</span></span>
<span data-ttu-id="ceeb0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceeb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ceeb0-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ceeb0-108">Permission type</span></span>      | <span data-ttu-id="ceeb0-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ceeb0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ceeb0-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ceeb0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ceeb0-111">Notes.ReadWrite, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceeb0-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="ceeb0-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ceeb0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceeb0-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ceeb0-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="ceeb0-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ceeb0-114">Application</span></span> | <span data-ttu-id="ceeb0-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceeb0-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ceeb0-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ceeb0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/onenote/pages/{id}/content
PATCH /users/{id | userPrincipalName}/onenote/pages/{id}/content
PATCH /groups/{id}/onenote/pages/{id}/content
PATCH /sites/{id}/onenote/pages/{id}/content
```
## <a name="request-headers"></a><span data-ttu-id="ceeb0-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ceeb0-117">Request headers</span></span>
| <span data-ttu-id="ceeb0-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ceeb0-118">Name</span></span>       | <span data-ttu-id="ceeb0-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ceeb0-119">Type</span></span> | <span data-ttu-id="ceeb0-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ceeb0-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ceeb0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ceeb0-121">Authorization</span></span>  | <span data-ttu-id="ceeb0-122">string</span><span class="sxs-lookup"><span data-stu-id="ceeb0-122">string</span></span>  | <span data-ttu-id="ceeb0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ceeb0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ceeb0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ceeb0-125">Content-Type</span></span> | <span data-ttu-id="ceeb0-126">string</span><span class="sxs-lookup"><span data-stu-id="ceeb0-126">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="ceeb0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ceeb0-127">Request body</span></span>
<span data-ttu-id="ceeb0-p103">В теле запроса укажите массив объектов [patchContentCommand](../resources/patchcontentcommand.md), представляющих изменения, вносимые в страницу. Дополнительные сведения и примеры см. в статье <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Обновление страниц OneNote</a>.</span><span class="sxs-lookup"><span data-stu-id="ceeb0-p103">In the request body, supply an array of [patchContentCommand](../resources/patchcontentcommand.md) objects that represent the changes to the page. For more information and examples, see <a href="https://msdn.microsoft.com/office/office365/howto/onenote-update-page">Update OneNote pages</a>.</span></span>

## <a name="response"></a><span data-ttu-id="ceeb0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ceeb0-130">Response</span></span>

<span data-ttu-id="ceeb0-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`.  Для запроса PATCH не возвращается никаких данных JSON.</span><span class="sxs-lookup"><span data-stu-id="ceeb0-p104">If successful, this method returns a `204 No Content` response code.  No JSON data is returned for a PATCH request.</span></span>
## <a name="example"></a><span data-ttu-id="ceeb0-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ceeb0-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ceeb0-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ceeb0-134">Request</span></span>
<span data-ttu-id="ceeb0-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ceeb0-135">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="ceeb0-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="ceeb0-136">Response</span></span>
<span data-ttu-id="ceeb0-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ceeb0-137">Here is an example of the response.</span></span> 
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
