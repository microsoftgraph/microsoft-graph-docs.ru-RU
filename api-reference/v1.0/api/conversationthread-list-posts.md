---
title: Список публикаций
description: 'Получение публикаций из указанной цепочки. Вы можете указать родительский сеанс связи и поток, или '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 53433d7051f699b3d1524186700440bed73d781a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442848"
---
# <a name="list-posts"></a><span data-ttu-id="5efc9-104">Список публикаций</span><span class="sxs-lookup"><span data-stu-id="5efc9-104">List posts</span></span>

<span data-ttu-id="5efc9-p102">Получение записей из указанного потока. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="5efc9-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="5efc9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5efc9-107">Permissions</span></span>
<span data-ttu-id="5efc9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5efc9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5efc9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5efc9-110">Permission type</span></span>      | <span data-ttu-id="5efc9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5efc9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5efc9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5efc9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5efc9-113">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="5efc9-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="5efc9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5efc9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5efc9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5efc9-115">Not supported.</span></span>    |
|<span data-ttu-id="5efc9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5efc9-116">Application</span></span> | <span data-ttu-id="5efc9-117">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="5efc9-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5efc9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5efc9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="5efc9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5efc9-119">Optional query parameters</span></span>
<span data-ttu-id="5efc9-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5efc9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5efc9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5efc9-121">Request headers</span></span>
| <span data-ttu-id="5efc9-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5efc9-122">Header</span></span>       | <span data-ttu-id="5efc9-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5efc9-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5efc9-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5efc9-124">Authorization</span></span>  | <span data-ttu-id="5efc9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5efc9-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5efc9-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5efc9-127">Request body</span></span>
<span data-ttu-id="5efc9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5efc9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5efc9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5efc9-129">Response</span></span>

<span data-ttu-id="5efc9-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5efc9-130">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5efc9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5efc9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5efc9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5efc9-132">Request</span></span>
<span data-ttu-id="5efc9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5efc9-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5efc9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="5efc9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5efc9-135">C#</span><span class="sxs-lookup"><span data-stu-id="5efc9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5efc9-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="5efc9-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5efc9-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5efc9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5efc9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="5efc9-138">Response</span></span>
<span data-ttu-id="5efc9-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5efc9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
