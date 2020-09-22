---
title: Список цепочек
description: Получение всех цепочек группы.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5a25ae865219dde471e1c8d467dac2d963056f66
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057626"
---
# <a name="list-threads"></a><span data-ttu-id="15c04-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="15c04-103">List threads</span></span>

<span data-ttu-id="15c04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15c04-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15c04-105">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="15c04-105">Get all the threads of a group.</span></span>

><span data-ttu-id="15c04-106">**Примечание:** Вы также можете [получить все потоки беседы](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="15c04-106">**Note:** You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="15c04-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15c04-107">Permissions</span></span>
<span data-ttu-id="15c04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15c04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15c04-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15c04-110">Permission type</span></span>      | <span data-ttu-id="15c04-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15c04-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15c04-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15c04-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15c04-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15c04-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="15c04-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15c04-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15c04-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15c04-115">Not supported.</span></span>    |
|<span data-ttu-id="15c04-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15c04-116">Application</span></span> | <span data-ttu-id="15c04-117">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15c04-117">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15c04-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15c04-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15c04-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="15c04-119">Optional query parameters</span></span>
<span data-ttu-id="15c04-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="15c04-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15c04-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15c04-121">Request headers</span></span>
| <span data-ttu-id="15c04-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15c04-122">Header</span></span>       | <span data-ttu-id="15c04-123">Значение</span><span class="sxs-lookup"><span data-stu-id="15c04-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="15c04-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15c04-124">Authorization</span></span>  | <span data-ttu-id="15c04-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15c04-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="15c04-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15c04-127">Request body</span></span>
<span data-ttu-id="15c04-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15c04-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15c04-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="15c04-129">Response</span></span>
<span data-ttu-id="15c04-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ConversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="15c04-130">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15c04-131">Пример</span><span class="sxs-lookup"><span data-stu-id="15c04-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="15c04-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="15c04-132">Request</span></span>
<span data-ttu-id="15c04-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15c04-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="15c04-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="15c04-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_get_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```
# <a name="c"></a>[<span data-ttu-id="15c04-135">C#</span><span class="sxs-lookup"><span data-stu-id="15c04-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15c04-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15c04-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15c04-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15c04-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15c04-138">Java</span><span class="sxs-lookup"><span data-stu-id="15c04-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-get-threads-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="15c04-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="15c04-139">Response</span></span>
<span data-ttu-id="15c04-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="15c04-140">The following is an example of the response.</span></span>
><span data-ttu-id="15c04-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15c04-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

