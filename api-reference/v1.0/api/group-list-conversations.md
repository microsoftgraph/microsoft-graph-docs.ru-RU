---
title: Список бесед
description: Получение списка бесед в этой группе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6077cf4032c19ee35e43b0f4a69b0f385fb455ae
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337309"
---
# <a name="list-conversations"></a><span data-ttu-id="36288-103">Список бесед</span><span class="sxs-lookup"><span data-stu-id="36288-103">List conversations</span></span>
<span data-ttu-id="36288-104">Получение списка объектов [conversation](../resources/conversation.md) в этой группе.</span><span class="sxs-lookup"><span data-stu-id="36288-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="36288-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36288-105">Permissions</span></span>
<span data-ttu-id="36288-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36288-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36288-108">Permission type</span></span>      | <span data-ttu-id="36288-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36288-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36288-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36288-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36288-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36288-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="36288-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36288-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36288-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36288-113">Not supported.</span></span>    |
|<span data-ttu-id="36288-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36288-114">Application</span></span> | <span data-ttu-id="36288-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36288-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36288-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36288-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36288-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="36288-117">Optional query parameters</span></span>
<span data-ttu-id="36288-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="36288-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36288-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36288-119">Request headers</span></span>
| <span data-ttu-id="36288-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="36288-120">Header</span></span>       | <span data-ttu-id="36288-121">Значение</span><span class="sxs-lookup"><span data-stu-id="36288-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="36288-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36288-122">Authorization</span></span>  | <span data-ttu-id="36288-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="36288-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="36288-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="36288-125">Request body</span></span>
<span data-ttu-id="36288-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36288-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36288-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="36288-127">Response</span></span>
<span data-ttu-id="36288-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="36288-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36288-129">Пример</span><span class="sxs-lookup"><span data-stu-id="36288-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="36288-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="36288-130">Request</span></span>
<span data-ttu-id="36288-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36288-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="36288-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="36288-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="36288-133">C#</span><span class="sxs-lookup"><span data-stu-id="36288-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36288-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36288-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="36288-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="36288-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="36288-136">Java</span><span class="sxs-lookup"><span data-stu-id="36288-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="36288-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="36288-137">Response</span></span>
<span data-ttu-id="36288-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="36288-138">The following is an example of the response.</span></span>
><span data-ttu-id="36288-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36288-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 262

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
