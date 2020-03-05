---
title: Удаление объекта conversationThread
description: Удаление объекта conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0f2d5f157c712ed76ebce77c68ac163236a5fdec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436414"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="956d3-103">Удаление объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="956d3-103">Delete conversationThread</span></span>

<span data-ttu-id="956d3-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="956d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="956d3-105">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="956d3-105">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="956d3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="956d3-106">Permissions</span></span>
<span data-ttu-id="956d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="956d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="956d3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="956d3-109">Permission type</span></span>      | <span data-ttu-id="956d3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="956d3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="956d3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="956d3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="956d3-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956d3-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="956d3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="956d3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="956d3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="956d3-114">Not supported.</span></span>    |
|<span data-ttu-id="956d3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="956d3-115">Application</span></span> | <span data-ttu-id="956d3-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="956d3-116">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="956d3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="956d3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="956d3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="956d3-118">Request headers</span></span>
| <span data-ttu-id="956d3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="956d3-119">Header</span></span>       | <span data-ttu-id="956d3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="956d3-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="956d3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="956d3-121">Authorization</span></span>  | <span data-ttu-id="956d3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="956d3-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="956d3-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="956d3-124">Request body</span></span>
<span data-ttu-id="956d3-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="956d3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="956d3-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="956d3-126">Response</span></span>

<span data-ttu-id="956d3-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="956d3-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="956d3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="956d3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="956d3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="956d3-130">Request</span></span>
<span data-ttu-id="956d3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="956d3-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="956d3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="956d3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
# <a name="c"></a>[<span data-ttu-id="956d3-133">C#</span><span class="sxs-lookup"><span data-stu-id="956d3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="956d3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="956d3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="956d3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="956d3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="956d3-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="956d3-136">Response</span></span>
<span data-ttu-id="956d3-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="956d3-137">Here is an example of the response.</span></span> 
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
