---
title: Список цепочек
description: Получение всех цепочек группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 59531b379700e308d78e52af22ba62813910cb21
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273495"
---
# <a name="list-threads"></a><span data-ttu-id="a918b-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="a918b-103">List threads</span></span>
<span data-ttu-id="a918b-104">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="a918b-104">Get all the threads of a group.</span></span>

><span data-ttu-id="a918b-105">Примечание. Вы также можете [получить все цепочки беседы](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="a918b-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a918b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a918b-106">Permissions</span></span>
<span data-ttu-id="a918b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a918b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a918b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a918b-109">Permission type</span></span>      | <span data-ttu-id="a918b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a918b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a918b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a918b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a918b-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a918b-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a918b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a918b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a918b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a918b-114">Not supported.</span></span>    |
|<span data-ttu-id="a918b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a918b-115">Application</span></span> | <span data-ttu-id="a918b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a918b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a918b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a918b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a918b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a918b-118">Optional query parameters</span></span>
<span data-ttu-id="a918b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a918b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a918b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a918b-120">Request headers</span></span>
| <span data-ttu-id="a918b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a918b-121">Header</span></span>       | <span data-ttu-id="a918b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a918b-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a918b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a918b-123">Authorization</span></span>  | <span data-ttu-id="a918b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a918b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a918b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a918b-126">Request body</span></span>
<span data-ttu-id="a918b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a918b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a918b-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="a918b-128">Response</span></span>
<span data-ttu-id="a918b-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ConversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a918b-129">If successful, this method returns a `200 OK` response code and collection of [ConversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a918b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a918b-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a918b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a918b-131">Request</span></span>
<span data-ttu-id="a918b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a918b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/threads
```

#### <a name="response"></a><span data-ttu-id="a918b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="a918b-133">Response</span></span>
<span data-ttu-id="a918b-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a918b-134">The following is an example of the response.</span></span>
><span data-ttu-id="a918b-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a918b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a918b-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a918b-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a918b-138">C#</span><span class="sxs-lookup"><span data-stu-id="a918b-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_threads-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a918b-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="a918b-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_threads-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="a918b-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a918b-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_threads-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-list-threads.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
