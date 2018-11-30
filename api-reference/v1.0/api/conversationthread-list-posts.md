---
title: Список записей
description: 'Получение публикаций из указанной цепочки. Можно указать родительский беседы и поток, или, '
ms.openlocfilehash: 35c4c178b02cb700ab21a324c29a4522203fad19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025972"
---
# <a name="list-posts"></a><span data-ttu-id="2b565-104">Список записей</span><span class="sxs-lookup"><span data-stu-id="2b565-104">List posts</span></span>

<span data-ttu-id="2b565-p102">Получение записей из указанного потока. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="2b565-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b565-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2b565-107">Permissions</span></span>
<span data-ttu-id="2b565-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b565-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b565-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2b565-110">Permission type</span></span>      | <span data-ttu-id="2b565-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2b565-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b565-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2b565-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2b565-113">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b565-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="2b565-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2b565-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b565-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2b565-115">Not supported.</span></span>    |
|<span data-ttu-id="2b565-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2b565-116">Application</span></span> | <span data-ttu-id="2b565-117">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b565-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b565-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2b565-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="2b565-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2b565-119">Optional query parameters</span></span>
<span data-ttu-id="2b565-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2b565-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2b565-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2b565-121">Request headers</span></span>
| <span data-ttu-id="2b565-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2b565-122">Header</span></span>       | <span data-ttu-id="2b565-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2b565-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2b565-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2b565-124">Authorization</span></span>  | <span data-ttu-id="2b565-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2b565-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2b565-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2b565-127">Request body</span></span>
<span data-ttu-id="2b565-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2b565-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b565-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2b565-129">Response</span></span>

<span data-ttu-id="2b565-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2b565-130">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2b565-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2b565-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b565-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2b565-132">Request</span></span>
<span data-ttu-id="2b565-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2b565-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts
```
##### <a name="response"></a><span data-ttu-id="2b565-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="2b565-134">Response</span></span>
<span data-ttu-id="2b565-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="2b565-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
