---
title: Удаление страницы
description: Удаление страницы OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: e2861baa5a2423983e0e5324932cc5465746ae37
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019847"
---
# <a name="delete-page"></a><span data-ttu-id="a9798-103">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="a9798-103">Delete page</span></span>

<span data-ttu-id="a9798-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9798-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9798-105">Удаление страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="a9798-105">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="a9798-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9798-106">Permissions</span></span>
<span data-ttu-id="a9798-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9798-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9798-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9798-109">Permission type</span></span>      | <span data-ttu-id="a9798-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9798-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9798-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9798-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a9798-112">Notes. ReadWrite, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a9798-112">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9798-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9798-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9798-114">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a9798-114">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="a9798-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9798-115">Application</span></span> | <span data-ttu-id="a9798-116">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9798-116">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9798-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9798-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a9798-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9798-118">Request headers</span></span>
| <span data-ttu-id="a9798-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a9798-119">Name</span></span>       | <span data-ttu-id="a9798-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a9798-120">Type</span></span> | <span data-ttu-id="a9798-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a9798-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a9798-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9798-122">Authorization</span></span>  | <span data-ttu-id="a9798-123">string</span><span class="sxs-lookup"><span data-stu-id="a9798-123">string</span></span>  | <span data-ttu-id="a9798-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9798-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a9798-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9798-126">Response</span></span>

<span data-ttu-id="a9798-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a9798-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9798-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a9798-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9798-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9798-130">Request</span></span>
<span data-ttu-id="a9798-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9798-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a9798-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9798-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/onenote/pages/{id}
```
# <a name="c"></a>[<span data-ttu-id="a9798-133">C#</span><span class="sxs-lookup"><span data-stu-id="a9798-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a9798-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9798-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a9798-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9798-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a9798-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9798-136">Response</span></span>
<span data-ttu-id="a9798-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a9798-137">Here is an example of the response.</span></span>
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


