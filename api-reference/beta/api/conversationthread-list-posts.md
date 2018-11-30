---
title: Список записей
description: 'Получение публикаций из указанной цепочки. Можно указать родительский беседы и поток, или, '
ms.openlocfilehash: 9253076a0232954acfdd1effad3fdb8084bba3fd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078292"
---
# <a name="list-posts"></a><span data-ttu-id="bed27-104">Список записей</span><span class="sxs-lookup"><span data-stu-id="bed27-104">List posts</span></span>

> <span data-ttu-id="bed27-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bed27-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bed27-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bed27-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bed27-p103">Получение записей из указанного потока. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="bed27-p103">Get the posts of the specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="bed27-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bed27-109">Permissions</span></span>
<span data-ttu-id="bed27-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bed27-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bed27-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bed27-112">Permission type</span></span>      | <span data-ttu-id="bed27-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bed27-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bed27-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bed27-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bed27-115">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bed27-115">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="bed27-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bed27-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bed27-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bed27-117">Not supported.</span></span>    |
|<span data-ttu-id="bed27-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bed27-118">Application</span></span> | <span data-ttu-id="bed27-119">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="bed27-119">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bed27-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bed27-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts
GET /groups/{id}/conversations/{id}/threads/{id}/posts

```
## <a name="optional-query-parameters"></a><span data-ttu-id="bed27-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bed27-121">Optional query parameters</span></span>
<span data-ttu-id="bed27-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="bed27-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bed27-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bed27-123">Request headers</span></span>
| <span data-ttu-id="bed27-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bed27-124">Header</span></span>       | <span data-ttu-id="bed27-125">Значение</span><span class="sxs-lookup"><span data-stu-id="bed27-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bed27-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bed27-126">Authorization</span></span>  | <span data-ttu-id="bed27-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bed27-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bed27-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bed27-129">Request body</span></span>
<span data-ttu-id="bed27-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bed27-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bed27-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bed27-131">Response</span></span>

<span data-ttu-id="bed27-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [Post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bed27-132">If successful, this method returns a `200 OK` response code and collection of [Post](../resources/post.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bed27-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bed27-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bed27-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bed27-134">Request</span></span>
<span data-ttu-id="bed27-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bed27-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts
```
##### <a name="response"></a><span data-ttu-id="bed27-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="bed27-136">Response</span></span>
<span data-ttu-id="bed27-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="bed27-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
