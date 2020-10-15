---
title: Вывод записи
description: 'Получение свойств и связей публикации в указанной цепочке. Вы можете указать и родительский элемент '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2ce4db0e0cf4b17245ad7ad0e84a45e4152d567f
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458327"
---
# <a name="get-post"></a><span data-ttu-id="dfc26-104">Вывод записи</span><span class="sxs-lookup"><span data-stu-id="dfc26-104">Get post</span></span>

<span data-ttu-id="dfc26-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfc26-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfc26-p102">Получение свойств и связей записи в указанной цепочке. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="dfc26-p102">Get the properties and relationships of a post in a specified thread. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span>

<span data-ttu-id="dfc26-108">Так как ресурс **POST** поддерживает [расширения](/graph/extensibility-overview), с помощью операции можно также `GET` получить настраиваемые свойства и данные расширения в экземпляре **POST** .</span><span class="sxs-lookup"><span data-stu-id="dfc26-108">Since the **post** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **post** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfc26-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dfc26-109">Permissions</span></span>
<span data-ttu-id="dfc26-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfc26-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfc26-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfc26-112">Permission type</span></span>      | <span data-ttu-id="dfc26-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfc26-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfc26-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfc26-114">Delegated (work or school account)</span></span> | <span data-ttu-id="dfc26-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfc26-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dfc26-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfc26-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfc26-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfc26-117">Not supported.</span></span>    |
|<span data-ttu-id="dfc26-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="dfc26-118">Application</span></span> | <span data-ttu-id="dfc26-119">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfc26-119">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfc26-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfc26-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dfc26-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dfc26-121">Optional query parameters</span></span>
<span data-ttu-id="dfc26-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dfc26-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dfc26-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dfc26-123">Request headers</span></span>
| <span data-ttu-id="dfc26-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dfc26-124">Header</span></span>       | <span data-ttu-id="dfc26-125">Значение</span><span class="sxs-lookup"><span data-stu-id="dfc26-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dfc26-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfc26-126">Authorization</span></span>  | <span data-ttu-id="dfc26-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfc26-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfc26-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dfc26-129">Request body</span></span>
<span data-ttu-id="dfc26-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dfc26-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfc26-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfc26-131">Response</span></span>

<span data-ttu-id="dfc26-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [post](../resources/post.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfc26-132">If successful, this method returns a `200 OK` response code and [post](../resources/post.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dfc26-133">Пример</span><span class="sxs-lookup"><span data-stu-id="dfc26-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfc26-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfc26-134">Request</span></span>
<span data-ttu-id="dfc26-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfc26-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dfc26-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfc26-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_post"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}
```
# <a name="c"></a>[<span data-ttu-id="dfc26-137">C#</span><span class="sxs-lookup"><span data-stu-id="dfc26-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfc26-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfc26-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfc26-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfc26-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfc26-140">Java</span><span class="sxs-lookup"><span data-stu-id="dfc26-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dfc26-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfc26-141">Response</span></span>
<span data-ttu-id="dfc26-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="dfc26-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="dfc26-145">См. также</span><span class="sxs-lookup"><span data-stu-id="dfc26-145">See also</span></span>

- [<span data-ttu-id="dfc26-146">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="dfc26-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="dfc26-147">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="dfc26-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
