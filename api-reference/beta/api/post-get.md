---
title: Вывод записи
description: 'Получение свойств и связей публикации в указанной цепочке. Можно указать как родительской '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ecccee4f63136d43c375e648e9a073e489f99c17
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968591"
---
# <a name="get-post"></a><span data-ttu-id="e28ff-104">Вывод записи</span><span class="sxs-lookup"><span data-stu-id="e28ff-104">Get post</span></span>

> <span data-ttu-id="e28ff-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e28ff-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e28ff-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e28ff-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e28ff-p103">Получение свойств и связей записи в указанной цепочке. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="e28ff-p103">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="e28ff-109">Так как ресурс **post** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **post**.</span><span class="sxs-lookup"><span data-stu-id="e28ff-109">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="e28ff-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e28ff-110">Permissions</span></span>
<span data-ttu-id="e28ff-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e28ff-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e28ff-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e28ff-113">Permission type</span></span>      | <span data-ttu-id="e28ff-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e28ff-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e28ff-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e28ff-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e28ff-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e28ff-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e28ff-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e28ff-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e28ff-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e28ff-118">Not supported.</span></span>    |
|<span data-ttu-id="e28ff-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e28ff-119">Application</span></span> | <span data-ttu-id="e28ff-120">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e28ff-120">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e28ff-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e28ff-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e28ff-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e28ff-122">Optional query parameters</span></span>
<span data-ttu-id="e28ff-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e28ff-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e28ff-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e28ff-124">Request headers</span></span>
| <span data-ttu-id="e28ff-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e28ff-125">Header</span></span>       | <span data-ttu-id="e28ff-126">Значение</span><span class="sxs-lookup"><span data-stu-id="e28ff-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e28ff-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e28ff-127">Authorization</span></span>  | <span data-ttu-id="e28ff-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e28ff-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e28ff-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e28ff-130">Request body</span></span>
<span data-ttu-id="e28ff-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e28ff-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e28ff-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e28ff-132">Response</span></span>

<span data-ttu-id="e28ff-133">В случае успеха этот метод возвращает код отклика `200 OK` и объект [post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e28ff-133">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e28ff-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e28ff-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e28ff-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e28ff-135">Request</span></span>
<span data-ttu-id="e28ff-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e28ff-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
##### <a name="response"></a><span data-ttu-id="e28ff-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="e28ff-137">Response</span></span>
<span data-ttu-id="e28ff-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e28ff-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e28ff-141">См. также</span><span class="sxs-lookup"><span data-stu-id="e28ff-141">See also</span></span>

- [<span data-ttu-id="e28ff-142">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="e28ff-142">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e28ff-143">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e28ff-143">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e28ff-144">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e28ff-144">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
