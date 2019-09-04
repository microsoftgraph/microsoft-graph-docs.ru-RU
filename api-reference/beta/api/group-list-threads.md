---
title: Список цепочек
description: Получение всех цепочек группы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 6eaa699ce343043f0f5af2446f8faa1f482581d0
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721567"
---
# <a name="list-threads"></a><span data-ttu-id="44d53-103">Список цепочек</span><span class="sxs-lookup"><span data-stu-id="44d53-103">List threads</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44d53-104">Получение всех цепочек группы.</span><span class="sxs-lookup"><span data-stu-id="44d53-104">Get all the threads of a group.</span></span>

<span data-ttu-id="44d53-105">Примечание. Вы также можете [получить все цепочки беседы](conversation-list-threads.md).</span><span class="sxs-lookup"><span data-stu-id="44d53-105">Note: You can also [get all the threads of a conversation](conversation-list-threads.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="44d53-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="44d53-106">Permissions</span></span>
<span data-ttu-id="44d53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44d53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44d53-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44d53-109">Permission type</span></span>      | <span data-ttu-id="44d53-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="44d53-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44d53-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44d53-111">Delegated (work or school account)</span></span> | <span data-ttu-id="44d53-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d53-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="44d53-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44d53-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44d53-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44d53-114">Not supported.</span></span>    |
|<span data-ttu-id="44d53-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44d53-115">Application</span></span> | <span data-ttu-id="44d53-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44d53-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44d53-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44d53-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44d53-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="44d53-118">Optional query parameters</span></span>
<span data-ttu-id="44d53-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="44d53-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44d53-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="44d53-120">Request headers</span></span>
| <span data-ttu-id="44d53-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44d53-121">Header</span></span>       | <span data-ttu-id="44d53-122">Значение</span><span class="sxs-lookup"><span data-stu-id="44d53-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="44d53-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="44d53-123">Authorization</span></span>  | <span data-ttu-id="44d53-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44d53-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44d53-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="44d53-126">Request body</span></span>
<span data-ttu-id="44d53-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="44d53-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44d53-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="44d53-128">Response</span></span>
<span data-ttu-id="44d53-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [conversationThread](../resources/conversationthread.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="44d53-129">If successful, this method returns a `200 OK` response code and collection of [conversationThread](../resources/conversationthread.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44d53-130">Пример</span><span class="sxs-lookup"><span data-stu-id="44d53-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="44d53-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="44d53-131">Request</span></span>
<span data-ttu-id="44d53-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44d53-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="44d53-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="44d53-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_threads"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/threads
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44d53-134">C#</span><span class="sxs-lookup"><span data-stu-id="44d53-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-threads-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44d53-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="44d53-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-threads-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44d53-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="44d53-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-threads-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="44d53-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="44d53-137">Response</span></span>
<span data-ttu-id="44d53-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="44d53-138">The following is an example of the response.</span></span>
><span data-ttu-id="44d53-139">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="44d53-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="44d53-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44d53-140">All the properties will be returned from an actual call.</span></span>
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
      "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
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
<!--
{
  "type": "#page.annotation",
  "description": "List group threads",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
