---
title: Список бесед
description: Получение списка бесед в этой группе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5eed72701d0ecb4bbddc4ec3b90a6c0f94a7f810
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36420233"
---
# <a name="list-conversations"></a><span data-ttu-id="63f01-103">Список бесед</span><span class="sxs-lookup"><span data-stu-id="63f01-103">List conversations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63f01-104">Получение списка объектов [conversation](../resources/conversation.md) в этой группе.</span><span class="sxs-lookup"><span data-stu-id="63f01-104">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="63f01-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="63f01-105">Permissions</span></span>
<span data-ttu-id="63f01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63f01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63f01-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="63f01-108">Permission type</span></span>      | <span data-ttu-id="63f01-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="63f01-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63f01-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="63f01-110">Delegated (work or school account)</span></span> | <span data-ttu-id="63f01-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63f01-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="63f01-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="63f01-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63f01-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63f01-113">Not supported.</span></span>    |
|<span data-ttu-id="63f01-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="63f01-114">Application</span></span> | <span data-ttu-id="63f01-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63f01-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="63f01-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="63f01-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63f01-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="63f01-117">Optional query parameters</span></span>
<span data-ttu-id="63f01-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="63f01-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="63f01-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="63f01-119">Request headers</span></span>
| <span data-ttu-id="63f01-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="63f01-120">Header</span></span>       | <span data-ttu-id="63f01-121">Значение</span><span class="sxs-lookup"><span data-stu-id="63f01-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63f01-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="63f01-122">Authorization</span></span>  | <span data-ttu-id="63f01-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="63f01-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63f01-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="63f01-125">Request body</span></span>
<span data-ttu-id="63f01-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="63f01-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63f01-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="63f01-127">Response</span></span>
<span data-ttu-id="63f01-128">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="63f01-128">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63f01-129">Пример</span><span class="sxs-lookup"><span data-stu-id="63f01-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="63f01-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="63f01-130">Request</span></span>
<span data-ttu-id="63f01-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="63f01-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63f01-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="63f01-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/conversations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="63f01-133">C#</span><span class="sxs-lookup"><span data-stu-id="63f01-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63f01-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63f01-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63f01-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="63f01-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="63f01-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="63f01-136">Response</span></span>
<span data-ttu-id="63f01-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="63f01-137">The following is an example of the response.</span></span>
><span data-ttu-id="63f01-138">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63f01-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="63f01-139">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="63f01-139">All the properties will be returned from an actual call.</span></span>
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
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "List conversations",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
