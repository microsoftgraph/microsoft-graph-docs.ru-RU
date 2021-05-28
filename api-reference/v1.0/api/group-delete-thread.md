---
title: Удаление цепочки беседы
description: Удаление объекта thread.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 39f313f70923e34579596407472b9721dedb72b7
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681027"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="8fb61-103">Удаление цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="8fb61-103">Delete conversation thread</span></span>

<span data-ttu-id="8fb61-104">Пространство имен: microsoft.graph Delete a [thread](../resources/conversationthread.md) object.</span><span class="sxs-lookup"><span data-stu-id="8fb61-104">Namespace: microsoft.graph Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fb61-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8fb61-105">Permissions</span></span>
<span data-ttu-id="8fb61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fb61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fb61-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8fb61-108">Permission type</span></span>      | <span data-ttu-id="8fb61-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8fb61-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fb61-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8fb61-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8fb61-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fb61-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8fb61-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8fb61-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fb61-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fb61-113">Not supported.</span></span>    |
|<span data-ttu-id="8fb61-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8fb61-114">Application</span></span> | <span data-ttu-id="8fb61-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8fb61-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fb61-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8fb61-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8fb61-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8fb61-117">Request headers</span></span>
| <span data-ttu-id="8fb61-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8fb61-118">Name</span></span>       | <span data-ttu-id="8fb61-119">Тип</span><span class="sxs-lookup"><span data-stu-id="8fb61-119">Type</span></span> | <span data-ttu-id="8fb61-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8fb61-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8fb61-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fb61-121">Authorization</span></span>  | <span data-ttu-id="8fb61-122">string</span><span class="sxs-lookup"><span data-stu-id="8fb61-122">string</span></span>  | <span data-ttu-id="8fb61-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8fb61-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8fb61-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8fb61-125">Request body</span></span>
<span data-ttu-id="8fb61-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8fb61-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fb61-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fb61-127">Response</span></span>
<span data-ttu-id="8fb61-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8fb61-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fb61-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8fb61-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8fb61-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8fb61-131">Request</span></span>
<span data-ttu-id="8fb61-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8fb61-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8fb61-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8fb61-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315", "AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q=="],
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```
# <a name="c"></a>[<span data-ttu-id="8fb61-134">C#</span><span class="sxs-lookup"><span data-stu-id="8fb61-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-thread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8fb61-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fb61-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-thread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8fb61-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8fb61-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-thread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8fb61-137">Java</span><span class="sxs-lookup"><span data-stu-id="8fb61-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-thread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8fb61-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8fb61-138">Response</span></span>
<span data-ttu-id="8fb61-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8fb61-139">The following is an example of the response.</span></span> 
><span data-ttu-id="8fb61-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8fb61-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

