---
title: Список цепочек
description: Получение всех цепочек группы.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 75074f6602ac3c7b633a734dcf0ff3dc5c68ab1d
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43125171"
---
# <a name="list-threads"></a><span data-ttu-id="fa1f9-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="fa1f9-103">List threads</span></span>

<span data-ttu-id="fa1f9-104">Пространство имен: Microsoft. Graph — получение всех потоков группы.</span><span class="sxs-lookup"><span data-stu-id="fa1f9-104">Namespace: microsoft.graph Get all the threads of a group.</span></span>

><span data-ttu-id="fa1f9-105">Примечание. Вы также можете [получить все цепочки беседы](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="fa1f9-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa1f9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa1f9-106">Permissions</span></span>
<span data-ttu-id="fa1f9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa1f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa1f9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa1f9-109">Permission type</span></span>      | <span data-ttu-id="fa1f9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa1f9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa1f9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa1f9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fa1f9-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa1f9-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fa1f9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa1f9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa1f9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa1f9-114">Not supported.</span></span>    |
|<span data-ttu-id="fa1f9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa1f9-115">Application</span></span> | <span data-ttu-id="fa1f9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa1f9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa1f9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa1f9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa1f9-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fa1f9-118">Optional query parameters</span></span>
<span data-ttu-id="fa1f9-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fa1f9-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa1f9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa1f9-120">Request headers</span></span>
| <span data-ttu-id="fa1f9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa1f9-121">Header</span></span>       | <span data-ttu-id="fa1f9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fa1f9-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa1f9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa1f9-123">Authorization</span></span>  | <span data-ttu-id="fa1f9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa1f9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa1f9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fa1f9-126">Request body</span></span>
<span data-ttu-id="fa1f9-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fa1f9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa1f9-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="fa1f9-128">Response</span></span>
<span data-ttu-id="fa1f9-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ConversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fa1f9-129">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa1f9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fa1f9-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fa1f9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa1f9-131">Request</span></span>
<span data-ttu-id="fa1f9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa1f9-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fa1f9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fa1f9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="fa1f9-134">C#</span><span class="sxs-lookup"><span data-stu-id="fa1f9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fa1f9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa1f9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fa1f9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fa1f9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fa1f9-137">Java</span><span class="sxs-lookup"><span data-stu-id="fa1f9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fa1f9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa1f9-138">Response</span></span>
<span data-ttu-id="fa1f9-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa1f9-139">The following is an example of the response.</span></span>
><span data-ttu-id="fa1f9-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fa1f9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 536

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
