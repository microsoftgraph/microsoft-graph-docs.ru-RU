---
title: Получение объекта conversationThread
description: 'Получение определенной цепочки, принадлежащей группе. Вы можете указать родительский сеанс связи и поток, или '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7f63d088d3e202704d7bd22ff6e24b7db69b8d13
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721399"
---
# <a name="get-conversationthread"></a><span data-ttu-id="701e0-104">Получение conversationThread</span><span class="sxs-lookup"><span data-stu-id="701e0-104">Get conversationThread</span></span>

<span data-ttu-id="701e0-p102">Получение определенной цепочки, принадлежащей группе. Вы можете задать родительскую беседу вместе с цепочкой или только цепочку, не ссылаясь на родительскую беседу.</span><span class="sxs-lookup"><span data-stu-id="701e0-p102">Get a specific thread that belongs to a group. You can specify both the parent conversation and the thread, or, you can specify the thread without referencing the parent conversation.</span></span> 
## <a name="permissions"></a><span data-ttu-id="701e0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="701e0-107">Permissions</span></span>
<span data-ttu-id="701e0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="701e0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="701e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="701e0-110">Permission type</span></span>      | <span data-ttu-id="701e0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="701e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="701e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="701e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="701e0-113">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="701e0-113">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="701e0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="701e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="701e0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="701e0-115">Not supported.</span></span>    |
|<span data-ttu-id="701e0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="701e0-116">Application</span></span> | <span data-ttu-id="701e0-117">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="701e0-117">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="701e0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="701e0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}
GET /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="701e0-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="701e0-119">Optional query parameters</span></span>
<span data-ttu-id="701e0-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="701e0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="701e0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="701e0-121">Request headers</span></span>
| <span data-ttu-id="701e0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="701e0-122">Header</span></span>       | <span data-ttu-id="701e0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="701e0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="701e0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="701e0-124">Authorization</span></span>  | <span data-ttu-id="701e0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="701e0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="701e0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="701e0-127">Request body</span></span>
<span data-ttu-id="701e0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="701e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="701e0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="701e0-129">Response</span></span>

<span data-ttu-id="701e0-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="701e0-130">If successful, this method returns a `200 OK` response code and [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="701e0-131">Пример</span><span class="sxs-lookup"><span data-stu-id="701e0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="701e0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="701e0-132">Request</span></span>
<span data-ttu-id="701e0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="701e0-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="701e0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="701e0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="701e0-135">C#</span><span class="sxs-lookup"><span data-stu-id="701e0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversationthread-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="701e0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="701e0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversationthread-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="701e0-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="701e0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversationthread-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="701e0-138">Java</span><span class="sxs-lookup"><span data-stu-id="701e0-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversationthread-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="701e0-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="701e0-139">Response</span></span>
<span data-ttu-id="701e0-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="701e0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
