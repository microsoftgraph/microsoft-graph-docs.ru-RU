---
title: Вывод записи
description: 'Получение свойств и связей публикации в указанной цепочке. Можно указать как родительской '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0d786734aa59d0048b077d4fa7eae08857da2753
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514014"
---
# <a name="get-post"></a><span data-ttu-id="fbf38-104">Вывод записи</span><span class="sxs-lookup"><span data-stu-id="fbf38-104">Get post</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fbf38-p102">Получение свойств и связей записи в указанной цепочке. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="fbf38-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="fbf38-107">Так как ресурс **post** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **post**.</span><span class="sxs-lookup"><span data-stu-id="fbf38-107">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="fbf38-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fbf38-108">Permissions</span></span>
<span data-ttu-id="fbf38-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbf38-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbf38-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbf38-111">Permission type</span></span>      | <span data-ttu-id="fbf38-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbf38-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbf38-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbf38-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fbf38-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbf38-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fbf38-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbf38-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbf38-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbf38-116">Not supported.</span></span>    |
|<span data-ttu-id="fbf38-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbf38-117">Application</span></span> | <span data-ttu-id="fbf38-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbf38-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbf38-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbf38-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fbf38-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fbf38-120">Optional query parameters</span></span>
<span data-ttu-id="fbf38-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fbf38-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fbf38-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fbf38-122">Request headers</span></span>
| <span data-ttu-id="fbf38-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbf38-123">Header</span></span>       | <span data-ttu-id="fbf38-124">Значение</span><span class="sxs-lookup"><span data-stu-id="fbf38-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fbf38-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fbf38-125">Authorization</span></span>  | <span data-ttu-id="fbf38-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbf38-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fbf38-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fbf38-128">Request body</span></span>
<span data-ttu-id="fbf38-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fbf38-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbf38-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbf38-130">Response</span></span>

<span data-ttu-id="fbf38-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fbf38-131">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fbf38-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fbf38-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fbf38-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbf38-133">Request</span></span>
<span data-ttu-id="fbf38-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbf38-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/beta/groups/0d75b8dc-c42d-44dd-890a-751a99c0589f/threads/AAQkAD8EJUmcWwTJi06Cew==/posts/AQMkADgAAAIJbQAAAA==
```
##### <a name="response"></a><span data-ttu-id="fbf38-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="fbf38-135">Response</span></span>
<span data-ttu-id="fbf38-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fbf38-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="fbf38-139">См. также</span><span class="sxs-lookup"><span data-stu-id="fbf38-139">See also</span></span>

- [<span data-ttu-id="fbf38-140">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="fbf38-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fbf38-141">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="fbf38-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="fbf38-142">Добавление пользовательских данных в ресурсы group с помощью расширений схемы (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="fbf38-142">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)


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
    "Error: /api-reference/beta/api/post-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
