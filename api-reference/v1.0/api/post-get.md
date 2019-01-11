---
title: Вывод записи
description: 'Получение свойств и связей публикации в указанной цепочке. Можно указать как родительской '
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 9644b4be1ac1a64274703aecddca257e5559759e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825328"
---
# <a name="get-post"></a><span data-ttu-id="108ad-104">Вывод записи</span><span class="sxs-lookup"><span data-stu-id="108ad-104">Get post</span></span>

<span data-ttu-id="108ad-p102">Получение свойств и связей записи в указанной цепочке. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="108ad-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="108ad-107">Так как ресурс **post** поддерживает [расширения](/graph/extensibility-overview), с помощью операции `GET` можно также получить настраиваемые свойства и данные расширения в экземпляре **post**.</span><span class="sxs-lookup"><span data-stu-id="108ad-107">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="108ad-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="108ad-108">Permissions</span></span>
<span data-ttu-id="108ad-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="108ad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="108ad-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="108ad-111">Permission type</span></span>      | <span data-ttu-id="108ad-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="108ad-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="108ad-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="108ad-113">Delegated (work or school account)</span></span> | <span data-ttu-id="108ad-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="108ad-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="108ad-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="108ad-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="108ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="108ad-116">Not supported.</span></span>    |
|<span data-ttu-id="108ad-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="108ad-117">Application</span></span> | <span data-ttu-id="108ad-118">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="108ad-118">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="108ad-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="108ad-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="108ad-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="108ad-120">Optional query parameters</span></span>
<span data-ttu-id="108ad-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="108ad-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="108ad-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="108ad-122">Request headers</span></span>
| <span data-ttu-id="108ad-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="108ad-123">Header</span></span>       | <span data-ttu-id="108ad-124">Значение</span><span class="sxs-lookup"><span data-stu-id="108ad-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="108ad-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="108ad-125">Authorization</span></span>  | <span data-ttu-id="108ad-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="108ad-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="108ad-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="108ad-128">Request body</span></span>
<span data-ttu-id="108ad-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="108ad-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="108ad-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="108ad-130">Response</span></span>

<span data-ttu-id="108ad-131">В случае успеха этот метод возвращает код отклика `200 OK` и объект [post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="108ad-131">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="108ad-132">Пример</span><span class="sxs-lookup"><span data-stu-id="108ad-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="108ad-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="108ad-133">Request</span></span>
<span data-ttu-id="108ad-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="108ad-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
##### <a name="response"></a><span data-ttu-id="108ad-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="108ad-135">Response</span></span>
<span data-ttu-id="108ad-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="108ad-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 414

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
  }
}
```

## <a name="see-also"></a><span data-ttu-id="108ad-139">См. также</span><span class="sxs-lookup"><span data-stu-id="108ad-139">See also</span></span>

- [<span data-ttu-id="108ad-140">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="108ad-140">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="108ad-141">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="108ad-141">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get post",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
