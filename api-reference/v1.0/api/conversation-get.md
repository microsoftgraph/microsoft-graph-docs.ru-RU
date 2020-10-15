---
title: Получение беседы
description: Получение свойств и связей объекта беседы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1a992984302e9847887813574b8783b4285315f2
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460623"
---
# <a name="get-conversation"></a><span data-ttu-id="1b79a-103">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="1b79a-103">Get conversation</span></span>

<span data-ttu-id="1b79a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b79a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b79a-105">Получение свойств и связей объекта беседы.</span><span class="sxs-lookup"><span data-stu-id="1b79a-105">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1b79a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b79a-106">Permissions</span></span>
<span data-ttu-id="1b79a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b79a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b79a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b79a-109">Permission type</span></span>      | <span data-ttu-id="1b79a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b79a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b79a-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b79a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1b79a-112">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="1b79a-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="1b79a-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b79a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b79a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b79a-114">Not supported.</span></span>    |
|<span data-ttu-id="1b79a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="1b79a-115">Application</span></span> | <span data-ttu-id="1b79a-116">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="1b79a-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b79a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b79a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="1b79a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1b79a-118">Optional query parameters</span></span>
<span data-ttu-id="1b79a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1b79a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1b79a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b79a-120">Request headers</span></span>
| <span data-ttu-id="1b79a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b79a-121">Header</span></span>       | <span data-ttu-id="1b79a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1b79a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1b79a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b79a-123">Authorization</span></span>  | <span data-ttu-id="1b79a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b79a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1b79a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b79a-126">Request body</span></span>
<span data-ttu-id="1b79a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b79a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b79a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b79a-128">Response</span></span>

<span data-ttu-id="1b79a-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversation](../resources/conversation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b79a-129">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b79a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1b79a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b79a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b79a-131">Request</span></span>
<span data-ttu-id="1b79a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b79a-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b79a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b79a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
# <a name="c"></a>[<span data-ttu-id="1b79a-134">C#</span><span class="sxs-lookup"><span data-stu-id="1b79a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b79a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b79a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b79a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b79a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b79a-137">Java</span><span class="sxs-lookup"><span data-stu-id="1b79a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1b79a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b79a-138">Response</span></span>
<span data-ttu-id="1b79a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b79a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "datetime-value",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
