---
title: Список цепочек
description: Получение всех цепочек в групповой беседе.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 432d2757d2cc5142fa2b8660ebf8bfcd649800fa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442918"
---
# <a name="list-threads"></a><span data-ttu-id="e73a0-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="e73a0-103">List threads</span></span>

<span data-ttu-id="e73a0-104">Получение всех цепочек в групповой беседе.</span><span class="sxs-lookup"><span data-stu-id="e73a0-104">Get all the threads in a group conversation.</span></span>

<span data-ttu-id="e73a0-105">Примечание. Вы также можете [получить все цепочки группы](group-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="e73a0-105">Note: You can also [get all the threads of a group](group-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e73a0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e73a0-106">Permissions</span></span>
<span data-ttu-id="e73a0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e73a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e73a0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e73a0-109">Permission type</span></span>      | <span data-ttu-id="e73a0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e73a0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e73a0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e73a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e73a0-112">Group. ReadWrite. ALL, Group. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="e73a0-112">Group.ReadWrite.All, Group.Read.All</span></span>    |
|<span data-ttu-id="e73a0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e73a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e73a0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e73a0-114">Not supported.</span></span>    |
|<span data-ttu-id="e73a0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e73a0-115">Application</span></span> | <span data-ttu-id="e73a0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e73a0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e73a0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e73a0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/conversations/{id}/threads
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e73a0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e73a0-118">Optional query parameters</span></span>
<span data-ttu-id="e73a0-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e73a0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e73a0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e73a0-120">Request headers</span></span>
| <span data-ttu-id="e73a0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e73a0-121">Header</span></span>       | <span data-ttu-id="e73a0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e73a0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e73a0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e73a0-123">Authorization</span></span>  | <span data-ttu-id="e73a0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e73a0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e73a0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e73a0-126">Request body</span></span>
<span data-ttu-id="e73a0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e73a0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e73a0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e73a0-128">Response</span></span>

<span data-ttu-id="e73a0-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e73a0-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e73a0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e73a0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e73a0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e73a0-131">Request</span></span>
<span data-ttu-id="e73a0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e73a0-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e73a0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e73a0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_threads"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e73a0-134">C#</span><span class="sxs-lookup"><span data-stu-id="e73a0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e73a0-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="e73a0-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e73a0-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e73a0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e73a0-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e73a0-137">Response</span></span>
<span data-ttu-id="e73a0-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e73a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
