---
title: Список публикаций
description: 'Получение публикаций из указанной цепочки. Можно указать родительский разговор и поток, или, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4f4905edd2e1f23a5eda9bf38aa64a9bf69aa7ee
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047016"
---
# <a name="list-posts"></a><span data-ttu-id="8b416-104">Список публикаций</span><span class="sxs-lookup"><span data-stu-id="8b416-104">List posts</span></span>

<span data-ttu-id="8b416-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b416-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b416-p102">Получение записей из указанного потока. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="8b416-p102">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b416-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b416-108">Permissions</span></span>
<span data-ttu-id="8b416-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b416-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b416-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b416-111">Permission type</span></span>      | <span data-ttu-id="8b416-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b416-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b416-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b416-113">Delegated (work or school account)</span></span> | <span data-ttu-id="8b416-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b416-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8b416-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b416-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b416-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b416-116">Not supported.</span></span>    |
|<span data-ttu-id="8b416-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8b416-117">Application</span></span> | <span data-ttu-id="8b416-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b416-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b416-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b416-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b416-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8b416-120">Optional query parameters</span></span>
<span data-ttu-id="8b416-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8b416-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8b416-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b416-122">Request headers</span></span>
| <span data-ttu-id="8b416-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b416-123">Header</span></span>       | <span data-ttu-id="8b416-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8b416-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b416-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b416-125">Authorization</span></span>  | <span data-ttu-id="8b416-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b416-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b416-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8b416-128">Request body</span></span>
<span data-ttu-id="8b416-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b416-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b416-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b416-130">Response</span></span>

<span data-ttu-id="8b416-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b416-131">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b416-132">Пример</span><span class="sxs-lookup"><span data-stu-id="8b416-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b416-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b416-133">Request</span></span>
<span data-ttu-id="8b416-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b416-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8b416-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b416-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
# <a name="c"></a>[<span data-ttu-id="8b416-136">C#</span><span class="sxs-lookup"><span data-stu-id="8b416-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b416-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b416-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b416-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b416-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b416-139">Java</span><span class="sxs-lookup"><span data-stu-id="8b416-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-posts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8b416-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b416-140">Response</span></span>
<span data-ttu-id="8b416-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b416-141">Here is an example of the response.</span></span> <span data-ttu-id="8b416-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8b416-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts",
    "value":[
        {
            "@odata.etag":"W/\"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK\"",
            "id":"AQMkADgAAAIJbQAAAA==",
            "createdDateTime":"2018-01-11T17:36:17Z",
            "lastModifiedDateTime":"2018-01-11T17:36:17Z",
            "importance": "normal",
            "changeKey":"CQAAABYAAAC/3QURwysWS6IJYYw5exv4AAAAAAlK",
            "categories":[

            ],
            "receivedDateTime":"2018-01-11T17:36:17Z",
            "hasAttachments":false,
            "body":{
                "contentType":"html",
                "content":"<html><body></body></html>"
            },
            "from":{
                "emailAddress":{
                    "name":"Marketing",
                    "address":"Marketing@M365B489948.onmicrosoft.com"
                }
            },
            "sender":{
                "emailAddress":{
                    "name":"Marketing",
                    "address":"Marketing@M365B489948.onmicrosoft.com"
                }
            }
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
