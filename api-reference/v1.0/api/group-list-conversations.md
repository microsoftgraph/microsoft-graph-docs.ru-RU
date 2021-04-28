---
title: Список бесед
description: Получение списка бесед в этой группе.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0cc953819cf1613654f3142a983172167c176ed9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052336"
---
# <a name="list-conversations"></a><span data-ttu-id="cc3c6-103">Список бесед</span><span class="sxs-lookup"><span data-stu-id="cc3c6-103">List conversations</span></span>

<span data-ttu-id="cc3c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc3c6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc3c6-105">Получение списка объектов [conversation](../resources/conversation.md) в этой группе.</span><span class="sxs-lookup"><span data-stu-id="cc3c6-105">Retrieve the list of [conversations](../resources/conversation.md) in this group.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc3c6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cc3c6-106">Permissions</span></span>
<span data-ttu-id="cc3c6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc3c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc3c6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cc3c6-109">Permission type</span></span>      | <span data-ttu-id="cc3c6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cc3c6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc3c6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cc3c6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc3c6-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3c6-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cc3c6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cc3c6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc3c6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc3c6-114">Not supported.</span></span>    |
|<span data-ttu-id="cc3c6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cc3c6-115">Application</span></span> | <span data-ttu-id="cc3c6-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc3c6-116">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc3c6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cc3c6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc3c6-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cc3c6-118">Optional query parameters</span></span>
<span data-ttu-id="cc3c6-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cc3c6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc3c6-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cc3c6-120">Request headers</span></span>
| <span data-ttu-id="cc3c6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cc3c6-121">Header</span></span>       | <span data-ttu-id="cc3c6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cc3c6-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc3c6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cc3c6-123">Authorization</span></span>  | <span data-ttu-id="cc3c6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc3c6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc3c6-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cc3c6-126">Request body</span></span>
<span data-ttu-id="cc3c6-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cc3c6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc3c6-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc3c6-128">Response</span></span>
<span data-ttu-id="cc3c6-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversation](../resources/conversation.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cc3c6-129">If successful, this method returns a `200 OK` response code and collection of [conversation](../resources/conversation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc3c6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cc3c6-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cc3c6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cc3c6-131">Request</span></span>
<span data-ttu-id="cc3c6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cc3c6-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc3c6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc3c6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversations"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations
```
# <a name="c"></a>[<span data-ttu-id="cc3c6-134">C#</span><span class="sxs-lookup"><span data-stu-id="cc3c6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc3c6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc3c6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc3c6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc3c6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc3c6-137">Java</span><span class="sxs-lookup"><span data-stu-id="cc3c6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cc3c6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cc3c6-138">Response</span></span>
<span data-ttu-id="cc3c6-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cc3c6-139">The following is an example of the response.</span></span>
><span data-ttu-id="cc3c6-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cc3c6-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

