---
title: Список публикаций
description: 'Получение публикаций из указанной цепочки. Вы можете указать родительский сеанс связи и поток, или '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 10029e37f59af0370432ebef2c3c3624667fd336
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518177"
---
# <a name="list-posts"></a><span data-ttu-id="5033e-104">Список публикаций</span><span class="sxs-lookup"><span data-stu-id="5033e-104">List posts</span></span>

<span data-ttu-id="5033e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5033e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5033e-p102">Получение записей из указанного потока. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="5033e-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="5033e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5033e-108">Permissions</span></span>
<span data-ttu-id="5033e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5033e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5033e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5033e-111">Permission type</span></span>      | <span data-ttu-id="5033e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5033e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5033e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5033e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5033e-114">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="5033e-114">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="5033e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5033e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5033e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5033e-116">Not supported.</span></span>    |
|<span data-ttu-id="5033e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5033e-117">Application</span></span> | <span data-ttu-id="5033e-118">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="5033e-118">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5033e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5033e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="5033e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5033e-120">Optional query parameters</span></span>
<span data-ttu-id="5033e-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5033e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5033e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5033e-122">Request headers</span></span>
| <span data-ttu-id="5033e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5033e-123">Header</span></span>       | <span data-ttu-id="5033e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5033e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5033e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5033e-125">Authorization</span></span>  | <span data-ttu-id="5033e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5033e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5033e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5033e-128">Request body</span></span>
<span data-ttu-id="5033e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5033e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5033e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="5033e-130">Response</span></span>

<span data-ttu-id="5033e-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5033e-131">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5033e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5033e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5033e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5033e-133">Request</span></span>
<span data-ttu-id="5033e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5033e-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5033e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5033e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
# <a name="c"></a>[<span data-ttu-id="5033e-136">C#</span><span class="sxs-lookup"><span data-stu-id="5033e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5033e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5033e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5033e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5033e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5033e-139">Java</span><span class="sxs-lookup"><span data-stu-id="5033e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-posts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5033e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5033e-140">Response</span></span>
<span data-ttu-id="5033e-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5033e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
