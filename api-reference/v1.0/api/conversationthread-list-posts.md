---
title: Список публикаций
description: 'Получение публикаций из указанной цепочки. Можно указать родительский разговор и поток, или, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e2e641a6524a08a328fe6cfb7b879a9b8fb5e09a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053232"
---
# <a name="list-posts"></a><span data-ttu-id="70900-104">Список публикаций</span><span class="sxs-lookup"><span data-stu-id="70900-104">List posts</span></span>

<span data-ttu-id="70900-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70900-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70900-p102">Получение записей из указанного потока. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="70900-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="70900-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70900-108">Permissions</span></span>
<span data-ttu-id="70900-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70900-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70900-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70900-111">Permission type</span></span>      | <span data-ttu-id="70900-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70900-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70900-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70900-113">Delegated (work or school account)</span></span> | <span data-ttu-id="70900-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70900-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="70900-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70900-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70900-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70900-116">Not supported.</span></span>    |
|<span data-ttu-id="70900-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="70900-117">Application</span></span> | <span data-ttu-id="70900-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70900-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70900-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70900-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="70900-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="70900-120">Optional query parameters</span></span>
<span data-ttu-id="70900-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="70900-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="70900-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70900-122">Request headers</span></span>
| <span data-ttu-id="70900-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70900-123">Header</span></span>       | <span data-ttu-id="70900-124">Значение</span><span class="sxs-lookup"><span data-stu-id="70900-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70900-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70900-125">Authorization</span></span>  | <span data-ttu-id="70900-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70900-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70900-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70900-128">Request body</span></span>
<span data-ttu-id="70900-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="70900-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70900-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="70900-130">Response</span></span>

<span data-ttu-id="70900-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="70900-131">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="70900-132">Пример</span><span class="sxs-lookup"><span data-stu-id="70900-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70900-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="70900-133">Request</span></span>
<span data-ttu-id="70900-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="70900-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="70900-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="70900-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
# <a name="c"></a>[<span data-ttu-id="70900-136">C#</span><span class="sxs-lookup"><span data-stu-id="70900-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70900-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70900-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70900-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70900-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70900-139">Java</span><span class="sxs-lookup"><span data-stu-id="70900-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-posts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="70900-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="70900-140">Response</span></span>
<span data-ttu-id="70900-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="70900-141">Here is an example of the response.</span></span> <span data-ttu-id="70900-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="70900-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
  "value": [
    {
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "receivedDateTime": "datetime-value",
      "hasAttachments": true,
      "from": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "sender": {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      },
      "conversationThreadId": "conversationThreadId-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
