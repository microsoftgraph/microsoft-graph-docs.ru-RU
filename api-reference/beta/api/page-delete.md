---
title: Удаление страницы
description: Удаление страницы OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: e58c3c5763b0ce40932f235640c7fbf193945b5f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456021"
---
# <a name="delete-page"></a><span data-ttu-id="1fbc4-103">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="1fbc4-103">Delete page</span></span>

<span data-ttu-id="1fbc4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fbc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fbc4-105">Удаление страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="1fbc4-105">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="1fbc4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1fbc4-106">Permissions</span></span>
<span data-ttu-id="1fbc4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fbc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fbc4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1fbc4-109">Permission type</span></span>      | <span data-ttu-id="1fbc4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1fbc4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fbc4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1fbc4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1fbc4-112">Notes. ReadWrite, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="1fbc4-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1fbc4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1fbc4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fbc4-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1fbc4-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1fbc4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1fbc4-115">Application</span></span> | <span data-ttu-id="1fbc4-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fbc4-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fbc4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1fbc4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1fbc4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1fbc4-118">Request headers</span></span>
| <span data-ttu-id="1fbc4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1fbc4-119">Name</span></span>       | <span data-ttu-id="1fbc4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1fbc4-120">Type</span></span> | <span data-ttu-id="1fbc4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1fbc4-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1fbc4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fbc4-122">Authorization</span></span>  | <span data-ttu-id="1fbc4-123">string</span><span class="sxs-lookup"><span data-stu-id="1fbc4-123">string</span></span>  | <span data-ttu-id="1fbc4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1fbc4-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1fbc4-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1fbc4-126">Response</span></span>

<span data-ttu-id="1fbc4-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1fbc4-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fbc4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1fbc4-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1fbc4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1fbc4-130">Request</span></span>
<span data-ttu-id="1fbc4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1fbc4-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1fbc4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fbc4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
# <a name="c"></a>[<span data-ttu-id="1fbc4-133">C#</span><span class="sxs-lookup"><span data-stu-id="1fbc4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fbc4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fbc4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fbc4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fbc4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1fbc4-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="1fbc4-136">Response</span></span>
<span data-ttu-id="1fbc4-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1fbc4-137">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
