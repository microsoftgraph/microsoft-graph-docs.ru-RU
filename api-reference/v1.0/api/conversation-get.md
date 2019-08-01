---
title: Получение беседы
description: Получение свойств и связей объекта беседы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7661ceba1ef5719e2cc1711b1126771c40a4ebec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36003114"
---
# <a name="get-conversation"></a><span data-ttu-id="c91da-103">Получение беседы</span><span class="sxs-lookup"><span data-stu-id="c91da-103">Get conversation</span></span>

<span data-ttu-id="c91da-104">Получение свойств и связей объекта беседы.</span><span class="sxs-lookup"><span data-stu-id="c91da-104">Retrieve the properties and relationships of conversation object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c91da-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c91da-105">Permissions</span></span>
<span data-ttu-id="c91da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c91da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c91da-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c91da-108">Permission type</span></span>      | <span data-ttu-id="c91da-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c91da-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c91da-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c91da-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c91da-111">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c91da-111">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="c91da-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c91da-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c91da-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c91da-113">Not supported.</span></span>    |
|<span data-ttu-id="c91da-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c91da-114">Application</span></span> | <span data-ttu-id="c91da-115">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="c91da-115">Group.ReadWrite.All, Group.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c91da-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c91da-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}

```
## <a name="optional-query-parameters"></a><span data-ttu-id="c91da-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c91da-117">Optional query parameters</span></span>
<span data-ttu-id="c91da-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c91da-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c91da-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c91da-119">Request headers</span></span>
| <span data-ttu-id="c91da-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c91da-120">Header</span></span>       | <span data-ttu-id="c91da-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c91da-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c91da-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c91da-122">Authorization</span></span>  | <span data-ttu-id="c91da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c91da-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c91da-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c91da-125">Request body</span></span>
<span data-ttu-id="c91da-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c91da-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c91da-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c91da-127">Response</span></span>

<span data-ttu-id="c91da-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversation](../resources/conversation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c91da-128">If successful, this method returns a `200 OK` response code and [conversation](../resources/conversation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c91da-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c91da-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c91da-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c91da-130">Request</span></span>
<span data-ttu-id="c91da-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c91da-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c91da-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c91da-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c91da-133">C#</span><span class="sxs-lookup"><span data-stu-id="c91da-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c91da-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="c91da-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c91da-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c91da-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c91da-136">Java</span><span class="sxs-lookup"><span data-stu-id="c91da-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c91da-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c91da-137">Response</span></span>
<span data-ttu-id="c91da-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c91da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
