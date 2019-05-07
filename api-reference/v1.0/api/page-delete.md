---
title: Удаление страницы
description: Удаление страницы OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: a0b491c1b72920cbe30b4c7b65c11f7727f88049
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611337"
---
# <a name="delete-page"></a><span data-ttu-id="e7021-103">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="e7021-103">Delete page</span></span>

<span data-ttu-id="e7021-104">Удаление страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="e7021-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="e7021-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7021-105">Permissions</span></span>
<span data-ttu-id="e7021-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7021-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7021-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7021-108">Permission type</span></span>      | <span data-ttu-id="e7021-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7021-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7021-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7021-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7021-111">Notes. ReadWrite, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e7021-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e7021-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7021-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7021-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e7021-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e7021-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e7021-114">Application</span></span> | <span data-ttu-id="e7021-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7021-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7021-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7021-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e7021-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e7021-117">Request headers</span></span>
| <span data-ttu-id="e7021-118">Имя</span><span class="sxs-lookup"><span data-stu-id="e7021-118">Name</span></span>       | <span data-ttu-id="e7021-119">Тип</span><span class="sxs-lookup"><span data-stu-id="e7021-119">Type</span></span> | <span data-ttu-id="e7021-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e7021-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e7021-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7021-121">Authorization</span></span>  | <span data-ttu-id="e7021-122">string</span><span class="sxs-lookup"><span data-stu-id="e7021-122">string</span></span>  | <span data-ttu-id="e7021-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e7021-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e7021-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7021-125">Response</span></span>

<span data-ttu-id="e7021-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e7021-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7021-128">Пример</span><span class="sxs-lookup"><span data-stu-id="e7021-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7021-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7021-129">Request</span></span>
<span data-ttu-id="e7021-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e7021-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
##### <a name="response"></a><span data-ttu-id="e7021-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7021-131">Response</span></span>
<span data-ttu-id="e7021-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e7021-132">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e7021-133">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="e7021-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e7021-134">Языках</span><span class="sxs-lookup"><span data-stu-id="e7021-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_page-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7021-135">Язык</span><span class="sxs-lookup"><span data-stu-id="e7021-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_page-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/page-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/page-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
