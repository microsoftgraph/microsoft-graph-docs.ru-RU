---
title: Удаление цепочки беседы
description: Удаление объекта thread.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f4da21812bf7fb77f1c377b8d26e6857302447c0
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681804"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="9f655-103">Удаление цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="9f655-103">Delete conversation thread</span></span>

<span data-ttu-id="9f655-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f655-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f655-105">Удаление объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="9f655-105">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f655-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f655-106">Permissions</span></span>
<span data-ttu-id="9f655-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f655-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f655-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f655-109">Permission type</span></span>      | <span data-ttu-id="9f655-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f655-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f655-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f655-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9f655-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f655-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9f655-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f655-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f655-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f655-114">Not supported.</span></span>    |
|<span data-ttu-id="9f655-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f655-115">Application</span></span> | <span data-ttu-id="9f655-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f655-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f655-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f655-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9f655-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f655-118">Request headers</span></span>
| <span data-ttu-id="9f655-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9f655-119">Name</span></span>       | <span data-ttu-id="9f655-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9f655-120">Type</span></span> | <span data-ttu-id="9f655-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9f655-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9f655-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f655-122">Authorization</span></span>  | <span data-ttu-id="9f655-123">string</span><span class="sxs-lookup"><span data-stu-id="9f655-123">string</span></span>  | <span data-ttu-id="9f655-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f655-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f655-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f655-126">Request body</span></span>
<span data-ttu-id="9f655-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9f655-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f655-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f655-128">Response</span></span>
<span data-ttu-id="9f655-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9f655-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f655-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9f655-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9f655-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f655-132">Request</span></span>
<span data-ttu-id="9f655-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f655-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9f655-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f655-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="c"></a>[<span data-ttu-id="9f655-135">C#</span><span class="sxs-lookup"><span data-stu-id="9f655-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f655-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f655-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f655-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f655-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f655-138">Java</span><span class="sxs-lookup"><span data-stu-id="9f655-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-thread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9f655-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f655-139">Response</span></span>
<span data-ttu-id="9f655-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f655-140">The following is an example of the response.</span></span> 
><span data-ttu-id="9f655-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9f655-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


