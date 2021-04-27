---
title: Получение беседы
description: Получение свойств и связей объекта беседы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 937ad1e434f01716fbbd6c5634fbd60716f2a2c6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047044"
---
# <a name="get-conversation"></a><span data-ttu-id="00a0f-103">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="00a0f-103">Get conversation</span></span>

<span data-ttu-id="00a0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00a0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00a0f-105">Получение свойств и связей объекта беседы.</span><span class="sxs-lookup"><span data-stu-id="00a0f-105">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="00a0f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00a0f-106">Permissions</span></span>
<span data-ttu-id="00a0f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00a0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00a0f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00a0f-109">Permission type</span></span>      | <span data-ttu-id="00a0f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00a0f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00a0f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00a0f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00a0f-112">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="00a0f-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="00a0f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00a0f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00a0f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00a0f-114">Not supported.</span></span>    |
|<span data-ttu-id="00a0f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="00a0f-115">Application</span></span> | <span data-ttu-id="00a0f-116">Group.ReadWrite.All, Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="00a0f-116">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00a0f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00a0f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="00a0f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="00a0f-118">Optional query parameters</span></span>
<span data-ttu-id="00a0f-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="00a0f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="00a0f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00a0f-120">Request headers</span></span>
| <span data-ttu-id="00a0f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00a0f-121">Header</span></span>       | <span data-ttu-id="00a0f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00a0f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00a0f-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00a0f-123">Authorization</span></span>  | <span data-ttu-id="00a0f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00a0f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00a0f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00a0f-126">Request body</span></span>
<span data-ttu-id="00a0f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00a0f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00a0f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="00a0f-128">Response</span></span>

<span data-ttu-id="00a0f-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversation](../resources/conversation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00a0f-129">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00a0f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="00a0f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00a0f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="00a0f-131">Request</span></span>
<span data-ttu-id="00a0f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00a0f-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="00a0f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="00a0f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
# <a name="c"></a>[<span data-ttu-id="00a0f-134">C#</span><span class="sxs-lookup"><span data-stu-id="00a0f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00a0f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00a0f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00a0f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00a0f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00a0f-137">Java</span><span class="sxs-lookup"><span data-stu-id="00a0f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="00a0f-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="00a0f-138">Response</span></span>
<span data-ttu-id="00a0f-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00a0f-139">Here is an example of the response.</span></span> <span data-ttu-id="00a0f-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="00a0f-140">Note: The response object shown here might be shortened for readability.</span></span>
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
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "preview": "preview-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
