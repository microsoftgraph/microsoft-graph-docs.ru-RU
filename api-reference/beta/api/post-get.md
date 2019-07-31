---
title: Вывод записи
description: 'Получение свойств и связей публикации в указанной цепочке. Вы можете указать и родительский элемент '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f03251ecb6ba770bf2057ab95ecac91ab0d8f2c9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992075"
---
# <a name="get-post"></a><span data-ttu-id="ffafe-104">Вывод записи</span><span class="sxs-lookup"><span data-stu-id="ffafe-104">Get post</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffafe-p102">Получение свойств и связей записи в указанной цепочке. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="ffafe-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="ffafe-107">Так как ресурс **POST** поддерживает [расширения](/graph/extensibility-overview), с помощью `GET` операции можно также получить настраиваемые свойства и данные расширения в экземпляре **POST** .</span><span class="sxs-lookup"><span data-stu-id="ffafe-107">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffafe-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffafe-108">Permissions</span></span>
<span data-ttu-id="ffafe-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffafe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffafe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffafe-111">Permission type</span></span>      | <span data-ttu-id="ffafe-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffafe-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffafe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffafe-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ffafe-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffafe-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ffafe-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffafe-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffafe-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffafe-116">Not supported.</span></span>    |
|<span data-ttu-id="ffafe-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffafe-117">Application</span></span> | <span data-ttu-id="ffafe-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffafe-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffafe-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffafe-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ffafe-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ffafe-120">Optional query parameters</span></span>
<span data-ttu-id="ffafe-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ffafe-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ffafe-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffafe-122">Request headers</span></span>
| <span data-ttu-id="ffafe-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffafe-123">Header</span></span>       | <span data-ttu-id="ffafe-124">Значение</span><span class="sxs-lookup"><span data-stu-id="ffafe-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ffafe-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffafe-125">Authorization</span></span>  | <span data-ttu-id="ffafe-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffafe-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffafe-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ffafe-128">Request body</span></span>
<span data-ttu-id="ffafe-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffafe-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffafe-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffafe-130">Response</span></span>

<span data-ttu-id="ffafe-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ffafe-131">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ffafe-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ffafe-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ffafe-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffafe-133">Request</span></span>
<span data-ttu-id="ffafe-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffafe-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ffafe-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ffafe-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ffafe-136">C#</span><span class="sxs-lookup"><span data-stu-id="ffafe-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ffafe-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="ffafe-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ffafe-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ffafe-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ffafe-139">Java</span><span class="sxs-lookup"><span data-stu-id="ffafe-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ffafe-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffafe-140">Response</span></span>
<span data-ttu-id="ffafe-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="ffafe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups('0d75b8dc-c42d-44dd-890a-751a99c0589f')/threads('AAQkAD8EJUmcWwTJi06Cew%3D%3D')/posts/$entity",
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
```

## <a name="see-also"></a><span data-ttu-id="ffafe-144">См. также</span><span class="sxs-lookup"><span data-stu-id="ffafe-144">See also</span></span>

- [<span data-ttu-id="ffafe-145">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="ffafe-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ffafe-146">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ffafe-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ffafe-147">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ffafe-147">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
