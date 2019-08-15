---
title: Удаление объекта conversationThread
description: Удаление объекта conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f82a026cca65e1584cf4c46896ab0526622d5305
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417800"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="c86b4-103">Удаление объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="c86b4-103">Delete conversationThread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c86b4-104">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="c86b4-104">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="c86b4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c86b4-105">Permissions</span></span>
<span data-ttu-id="c86b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c86b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c86b4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c86b4-108">Permission type</span></span>      | <span data-ttu-id="c86b4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c86b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c86b4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c86b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c86b4-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c86b4-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c86b4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c86b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c86b4-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c86b4-113">Not supported.</span></span>    |
|<span data-ttu-id="c86b4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c86b4-114">Application</span></span> | <span data-ttu-id="c86b4-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c86b4-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c86b4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c86b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c86b4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c86b4-117">Request headers</span></span>
| <span data-ttu-id="c86b4-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c86b4-118">Header</span></span>       | <span data-ttu-id="c86b4-119">Значение</span><span class="sxs-lookup"><span data-stu-id="c86b4-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c86b4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c86b4-120">Authorization</span></span>  | <span data-ttu-id="c86b4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c86b4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c86b4-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c86b4-123">Request body</span></span>
<span data-ttu-id="c86b4-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c86b4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c86b4-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c86b4-125">Response</span></span>

<span data-ttu-id="c86b4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c86b4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c86b4-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c86b4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c86b4-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c86b4-129">Request</span></span>
<span data-ttu-id="c86b4-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c86b4-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c86b4-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c86b4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c86b4-132">C#</span><span class="sxs-lookup"><span data-stu-id="c86b4-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c86b4-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c86b4-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c86b4-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c86b4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c86b4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c86b4-135">Response</span></span>
<span data-ttu-id="c86b4-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c86b4-136">Here is an example of the response.</span></span> 
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
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
